# Project_2

1) Requirements
Colab
No setup needed; the script installs thop on the fly.
Local (optional)
Python 3.9+
PyTorch + torchvision (CUDA if you want GPU)
scikit-learn
matplotlib
thop

Install (CUDA example; adjust to your setup):
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
pip install scikit-learn matplotlib thop

2) How to Run
A) Google Colab (recommended)
Run the single cell. It will:
Download CIFAR-10 automatically.
Train VGG19 with augmentation.
Evaluate baseline.
Prune (structured by default), evaluate, then fine-tune pruned model (optional).
Benchmark latency & throughput across batch sizes.
Save and display plots and verdict tables.

B) Local (script form)
Copy the large cell code into a .py script (e.g., run_vgg19_prune.py).
Comment out Colab-specific bits (display(Image(...))).
Run:
python run_vgg19_prune.py
