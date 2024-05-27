# optimise-my-whisper

A very quick repo to showcase how you can experiment with Whisper (via Transformers) and make it run for your own use-cases!

All the experiments were run on a free Google Colab T4! 🔥 

Results and Colab below:

| **Method**                                    | **Time to Transcribe** |
|-----------------------------------------------|------------------------|
| fp16                                          | 62s                    |
| fp16 + SDPA                                   | 60s                    |
| fp16 + SDPA + Speculative Decoding            | 37.9s                  |
| fp16 + SDPA + Chunking + Speculative Decoding | 43.8s                  |
| Distil-whisper + fp16 + SDPA + Chunking       | **17.2s**              |
