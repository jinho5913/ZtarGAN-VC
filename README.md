# ZeroShot StarGAN-VC

#### 모델 
ZeroShot Learning이 가능한 StarGAN-VC 제안
1. 소리의 고유 정보를 손상시킬 수 있는 MCEP 대신 Mel-Spectrogram을 사용하여 소리 정보 손실 최소화
2. `Speaker Encoder`를 통해 모든 화자의 고유한 소리의 특징 정보 반영
3. 기존 StarGAN-VC에서 사용한 Attribute vector를 `Speaker Encoder`를 사용하여 출력된 Embedding Vector로 대체 -> ZeroShot Learning 가능
4. StarGAN-VC의 Domain Classifier 단에서 (1)에서 생성된 Embedding Vector를 사용하도록 수정

#### Architecture
<img width="1064" alt="image" src="https://user-images.githubusercontent.com/87609200/215251458-c700db9a-3940-4da7-ad16-48a6295b754a.png">

#### Framework
<img width="1107" alt="image" src="https://user-images.githubusercontent.com/87609200/215251516-a4282223-ed7e-4b12-880b-533e8323df8d.png">


