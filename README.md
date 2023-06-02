
# ChatGPT를 사용한 추천시스템 (recommender system with ChatGPT)

##  Data
- https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

## 선제 조건
- openAI API 키 받기
https://platform.openai.com/account/api-keys 에서 발급받으실 수 있습니다.

**recommender system using ChatGPT**
- ChatGPT을 활용한 추천 시스템
해당 추천시스템은 ChatGPT를 사용하여 사용자의 쿼리에서 의도(추천, 설명, 조회)를 파악하고 의도에 맞게 영화를 추천해주거나 설명해주는 모델입니다.

- 로직  
1. 사용자 query 입력
2. 의도 파악 (chatGPT)
3. 간단한 소개 문구 생성 출력 (chatGPT)
4. 추천, 설명 
4-1. 추천 -> 코사인 유사도 기반 top k개 출력
4-2. 사용자가 추천받은 영화에 대한 설명 요청 시 -> 위의 1~4 과정 거쳐 top1= 추천받은 영화에 대하여 설명함.

- 결과 화면    
![결과](https://github.com/baebae-dev/ChatGPT_recsys/assets/52961872/f32d8e05-a96c-433a-92a6-66cc241c3f18)

