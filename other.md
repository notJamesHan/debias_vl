macbook m2, needed to use python 3.8 due to arm.

environments
```
pyenv install 3.8.20
$(pyenv which python) -m venv debias
source debias/bin/activate
```

install
```
pip install https://download.pytorch.org/whl/cpu/torch-1.10.1-cp38-none-macosx_11_0_arm64.whl
pip install https://download.pytorch.org/whl/cpu/torchvision-0.13.0-cp38-cp38-macosx_11_0_arm64.whl#sha256=42d95ab197d090efc5669fec02fbc603d05c859e50ca2c60180d1a113aa9b3e2
pip install https://download.pytorch.org/whl/cpu/torchaudio-0.12.0-cp38-cp38-macosx_11_0_arm64.whl#sha256=d176ace6903bf5d1f57fea4a36aa37e6c848aa197c3d06d238dcae8831c92cbe``
pip install --upgrade torch torchvision
```


```
  deprecate("config-passed-as-path", "1.0.0", deprecation_message, standard_warn=False)
scheduler/scheduler_config.json: 100%|████████████████████████████████████████████████████| 346/346 [00:00<00:00, 248kB/s]
Traceback (most recent call last):
  File "/Users/jameshan/Documents/github/debias_vl/generative/main.py", line 133, in <module>
    P = torch.tensor(P).cuda()
  File "/Users/jameshan/Documents/github/debias_vl/debias/lib/python3.8/site-packages/torch/cuda/__init__.py", line 305, in _lazy_init
    raise AssertionError("Torch not compiled with CUDA enabled")
AssertionError: Torch not compiled with CUDA enabled
```