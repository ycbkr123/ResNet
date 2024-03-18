# ResNet-python
ResNet모델을 공부하기 위해 사용한 코드입니다.
해당 https://github.com/pytorch/vision/blob/6db1569c89094cf23f3bc41f79275c45e9fcb3f3/torchvision/models/resnet.py 참고하여 사용했습니다.

![image](https://github.com/ycbkr123/ResNet/assets/73626645/2356ac1d-cf17-4743-a933-b932e536afc6)

# ResNet
ResNet은 깊어진 신경망을 효과적으로 학습하기 위한 방법으로, residual 개념을 고안한 모델이다. 네트워크 깊이가 깊어질수록 성능이 좋아지다가 어느 시점에서 오히려 성능이 나빠지는데, 이러한 문제 해결을 위해 residual block을 도입했다. residual block은 기울기가 잘 전파될 수 있도록 하는 일종의 shortcut(skip connection)을 만들어 준다.
block은 계층의 묶음, 즉 합성곱층을 하나의 블록으로 묶은 것이다. 다음 그림과 같이 색상별로 블록을 구분했는데, 이러한 계층이 하나의 residual block이다. 그리고 residual block을 여러 개 쌓은 것을 ResNet이라 한다.
