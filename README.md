# Optimized_GPT2
Optimized GPT2 architecture to train a similar quality model in half the time

Running some experiments on RTX5090 rented on runpod

Multi-Head Attention (fp32):
Training completed in 4.88 minutes.

Multi-Head Attention + Matmul precision "high" (tf32):
Training completed in 3.34 minutes.

Multi-Head Attention + autocast (bf16):
Training completed in 2.64 minutes.

Multi-Head Attention + autocast (bf16) + torch.compile:
Training completed in 2.64 minutes.

Flash Attention + autocast (bf16) + torch.compile:
Training completed in 2.13 minutes.