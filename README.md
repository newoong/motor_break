# motor_break
Classify motor break - (interturn  fault / phase to phase fault)


## MLSTM-FCN
다변량 데이터를 다룰수 있는 시계열 분류 모델 MLSTM_FCN을 이용

1.다른 종류의 모터 고장 interturn falut 와 phase to phase fault 두가지 + 정상 모터 데이터, 총 3가지로 다중분류

2.특정 고장이 발생한 시계열 데이터에 대해서 정상, 고장 전 전조증상, 고장 발생 이후, 총 3가지로 다중 분류

-- 전조증상 부분 데이터 매우 짧음 -> 데이터 불균형 -> TimeGAN을 이용하여 임의의 전조증상 데이터 다량 생성하여 모델링

-- tsaug의 augmentation 기법들을 이용하여 test set 생성
