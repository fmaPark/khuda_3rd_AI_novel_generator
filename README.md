# khuda_3rd_AI_novel_generator

## 프로젝트 소개

'생성모델을 활용한 AI 소설 생성'은 생성 모델 KoAlpaca를 활용해 소설 창작에 특화된 인공지능을 개발하는 프로젝트입니다.

---

## 팀 소개
- 문지원
- 박민아

---

## 프로젝트 진행
### 데이터셋

- 위키문헌 "분류:단편소설"
- 네이버 블로그 "고전소설"

-> 총 2.7 MB

![KHUDA_3기_소설 생성 pptx (1)](https://github.com/Dyract/khuda_3rd_AI_novel_generator/assets/68277847/d07af4c4-0c1e-4887-a605-4e940377fb94)

- chatgpt를 활용한 현대어 문체 변환 진행

![KHUDA_3기_소설 생성 pptx (2)](https://github.com/Dyract/khuda_3rd_AI_novel_generator/assets/68277847/1a2be540-cdfc-4c59-8c82-f942a5a69156)

- 대사와 상황으로 분리된 csv파일 생성

---

### 모델 학습
- [KoAlpaca Polyglot-ko 12.8B](https://huggingface.co/beomi/KoAlpaca-Polyglot-12.8B)
- 학습 환경 : Colab pro+ V100 40GB
  
![KHUDA_3기_소설 생성 pptx (3)](https://github.com/Dyract/khuda_3rd_AI_novel_generator/assets/68277847/06de1fd8-2f9d-4234-9738-6fe80907a1a2)

- Instruction tuning 적용
  
![KHUDA_3기_소설 생성 pptx (4)](https://github.com/Dyract/khuda_3rd_AI_novel_generator/assets/68277847/a8c0ae1c-dbe7-48c3-a006-e1d802b4b92f)

- Efficient Fine tuning 활용

---

## 프로젝트 결과
### Example result

> 질문 : <br>
> 맥락 : '내가 하고 싶은 말은, 그러니까'<br>
> 답변 : 하고 부르며 손을 잡아 이끌어 앉으라고 하였다.  정주사는 떨리는 가슴을 두 손으로 붙잡고 자리에 앉았다.  그렇게 떨리는 목소리로 정주사는 말했다. 정주사는 다시 고개를 숙이고 한숨을 쉬며 말했다.   소리에 몸이 떨리기 시작했다   소리가 너무 크게 다가왔다  정주사는 떨리는 가슴을 두 손으로 붙잡고 자리에 앉았다. 정주사는 다시 고개를 숙이고 한숨을 쉬며 말했다.   이렇게 말하며   그렇게 떨리는 소리로 정주사는 말했다. 정주사는 떨리는 가슴을 두 손으로 붙잡고 자리에 앉았다. 정백수는 여전히   이렇게 말하며   이렇게 떨리는 소리로 정주사는 말했다.  백영감은 다시 고개를 숙이고   이렇게 떨리는 소리로 정주사는 말했다. 장골로 생긴 정백수는 몸도 크고 키도 컸지만 그의 몸은 가늘고 좁았다. 정백수는 가슴에 귀를 대고   이런 소리를 들으며   이렇게 떨리는 소리로 정백

> 질문 : <br>
> 맥락 : '멀리 떠났다. 느이 누나말이다.' <br>
> 답변: 내가 결혼을 하려고 했던 때, 우리 집이 너무 가난해지면서 동생의 학비 걱정 때문에 결혼을 하려던 내가 동생의 학비를 대줬다. 이것 때문에 나는 사랑하는 가족도 버리고 여기에 남아 있겠다고 했다. 우리 가족은 아버지의 사업 실패로 점점 어려워지던 그 해에 나를 버리고 서울로 나가려고 했었다. 하지만 결국 아버지는 병이 악화되고 어머니는 약값을 위해 내가 서울로 가는 것을 포기시켰다. 그래서 이 일이 발생했다......우리 아버지가 이렇게 고생하는 것을 생각하면 우리 가족은 어떻게 되어도 좋단 말이냐! 우리 아버지의 피 때문에 내가 그런 것은 사실이 아니야. 우리 가족이 어떻게 되어도 이런 짓을 한 건 아니야!'
