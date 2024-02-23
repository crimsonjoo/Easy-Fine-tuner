
# Easy Fine-tuner (for Beginner)

[![Open In Colab](https://img.shields.io/static/v1?label=Open%20in%20Colab&message=사용법&color=yellow&logo=googlecolab)](https://colab.research.google.com/drive/1J3I-Sx2juQO0Nb6nfy7i3uM7uXWZpNfu?hl=ko#scrollTo=SJ81RsG4QnFn)

&nbsp;



- Easy Fine-tuner는 sLLM 모델(7B~13B) 파인튜닝을 쉽고 빠르게 검증/시연하기 위한 환경을 제공합니다.
- (초심자 기준) Colab T4 GPU를 활용한 LoRA/Q-LoRA 파인튜닝 학습


&nbsp;



## Custom Dataset 추가방법

- 사용자 개인의 Dataset을 example-datasets 아래에 huggingface의 datasets 형식으로 저장시키면 dataset load가 쉽게 적용이 가능합니다.
- 자세한 방법은 위의 colab을 참고해 주세요.

&nbsp;
### Usage
```
git clone https://github.com/crimsonjoo/Easy-Fine-tuner.git
cd Easy-Fine-tuner
pip install -r requirements.txt
```

&nbsp;

## 주의사항
- 모든 Parameter는 Colab 무료 GPU(T4)에 최적화 되도록 설정했습니다.
- huggingface의 PEFT 패키지의 SFTTrainer, QLoRA를 사용합니다.
- 무료 GPU(T4)에 13B 가량 크기 모델을 사용하기 위해서 Double Quantization 기법을 사용했습니다.


&nbsp;
## Reference 
- https://github.com/lxe/simple-llm-finetuner
- https://github.com/choijhyeok/easy_finetuner
