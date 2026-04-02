# 2026학년도 봄학기 광주과학기술원 기계학습
## Quick Start
```pwsh
> python -m venv ml
> .\ml\Scripts\activate
> pip install -r .\requirements.txt
```

### Windows CUDA / Windows on ARM
윈도우에서 CUDA를 사용하거나 ARM을 사용 중이라면 별도의 인덱스를 명시해줘야 한다.  
> CUDA  
> > `https://download.pytorch.org/whl/cu130`  
> 
> Windows on ARM  
> > `https://download.pytorch.org/whl/cpu`  
> 
> 위의 인덱스를 PyTorch 설치 시 명시해야 한다.  
> 현재 시점에서 ARM 환경에서는 CUDA를 지원하지 않는다.  

`requirements.txt`에서 아래의 패키지를 삭제한 후 패키지 설치를 진행한다.  
```
torch
pytorch-lightning
torchmetrics
ISLP
```

이후 아래와 같이 PyTorch와 관련 패키지를 설치한다.  
```pwsh
> pip install torch --index-url {index_url}
> pip install pytorch-lightning torchmetrics ISLP
```
