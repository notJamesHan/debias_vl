Macbook M2, needed to use python 3.8 due to arm.

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

datasets
- Got waterbird dataaset from https://github.com/kohpangwei/group_DRO