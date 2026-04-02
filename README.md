# 2026학년도 봄학기 광주과학기술원 기계학습
## Quick Start
```pwsh
> python -m venv ml
> .\ml\Scripts\activate
> pip install -r .\requirements.txt
```

### Windows on ARM
파이썬의 기본 저장소인 PyPI에는 ARM용 PyTorch가 없다.  
따라서 이와 관련된 패키지는 별도로 설치해야 한다.  

`requirements.txt`에서 아래의 패키지를 삭제한 후 패키지 설치를 진행한다.  
```
torch==2.7
pytorch-lightning==2.6.1
torchmetrics==1.9.0
ISLP==0.4.1
```

이후 아래와 같이 PyTorch와 관련 패키지를 설치한다.  
```pwsh
> pip install torch==2.7 --index-url https://download.pytorch.org/whl/cpu
> pip install pytorch-lightning==2.6.1 torchmetrics==1.9.0 ISLP==0.4.1
```