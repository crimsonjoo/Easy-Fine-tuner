
# Easy Finetuner

[![Open In Colab](https://img.shields.io/static/v1?label=Open%20in%20Colab&message=사용법&color=yellow&logo=googlecolab)](https://colab.research.google.com/github/lxe/simple-llama-finetuner/blob/master/Simple_LLaMA_FineTuner.ipynb)


Easy Finetuner는 llama2 계열 모델의 fine-tune을 쉽게 사용하기 위해서 제작하였습니다. 

&nbsp;

## 주의사항

- 모든 Parameter는 colab T4 GPU에 최적화 되도록 설정했습니다. (만약 다른 GPU를 사용하고 싶다면 confing.py에서 fb16, bf16 을 사용하고자 하는 GPU에 맞게 변경해 주세요)
- huggingface의 PEFT 패키지의 SFTTrainer, lora를 사용합니다.
- 현재는 llama2 기반의 모델에만 적용가능하게 설정했습니다. (fine-tune, load, inference 모두)

&nbsp;
## Custom Dataset 추가방법

- 사용자 개인의 Dataset을 example-datasets 아래에 huggingface의 datasets 형식으로 저장시키면 dataset load가 쉽게 적용이 가능합니다.
- 자세한 방법은 위의 colab을 참고해 주세요.

&nbsp;
### Usage
```
git clone https://github.com/lxe/simple-llm-finetuner.git
cd simple-llm-finetuner
pip install -r requirements.txt
```

&nbsp;
## Reference 
- https://github.com/lxe/simple-llm-finetuner
