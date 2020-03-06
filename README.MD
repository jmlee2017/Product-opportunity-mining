# Social media mining for product planning: A product opportunity mining approach based on topic modeling and sentiment analysis
- **Abstract:** Social media data have recently attracted considerable attention as an emerging voice of the customer as it has rapidly become a channel for exchanging and storing customer-generated, large-scale, and unregulated voices about products. Although product planning studies using social media data have used systematic methods for product planning, their methods have limitations, such as the difficulty of identifying latent product features due to the use of only term-level analysis and insufficient consideration of opportunity potential analysis of the identified features. Therefore, an opportunity mining approach is proposed in this study to identify product opportunities based on topic modeling and sentiment analysis of social media data. For a multifunctional product, this approach can identify latent product topics discussed by product customers in social media using topic modeling, thereby quantifying the importance of each product topic. Next, the satisfaction level of each product topic is evaluated using sentiment analysis. Finally, the opportunity value and improvement direction of each product topic from a customer-centered view are identified by an opportunity algorithm based on product topics’ importance and satisfaction. We expect that our approach for product planning will contribute to the systematic identification of product opportunities from large-scale customer-generated social media data and will be used as a real-time monitoring tool for changing customer needs analysis in rapidly evolving product environments.
- **Link:** [https://www.sciencedirect.com/science/article/pii/S0268401217302955](https://www.sciencedirect.com/science/article/pii/S0268401217302955)
- **Cite:** Jeong, Byeongki, Janghyeok Yoon, and Jae-Min Lee. "Social media mining for product planning: A product opportunity mining approach based on topic modeling and sentiment analysis." International Journal of Information Management 48 (2019): 280-290.

## Data and Codes
- 1.data_and_preprocessing
  - body.txt: Galaxy note5 subreddit의 Posts 및 Comments 데이터 본문  
  - edgeList.txt: Alchemy API를 통한 키워드 추출 결과를 Edge list 형태로 정리한 것
  - edgeList.nmf: Netminer를 이용한 Topic modeling을 위해 상기된 Edge list를 Netminer 형식으로 변경한 것 
- 1-1.alchemy: Alchemy API 사용을 위한 Visual studo (C#) project 
- 2.LDA_topic_modeling: Netminer를 이용한 Topic modeling 결과 (최적 토픽 수는 65개로 결정)
  - LDA_[R] Main.html
  - LDA_[T] Document Classification.csv
  - LDA_[T] SubNode Distribution over topic.csv
  - LDA_[T] Topic Distribution Over Mainnode.csv
  - LDA_[T] Topic Info.csv
- 3.Opportunity_algorithm
  - Topic_labeling.xlsx: 각 Topic의 상위 키워드를 이용하여 해석한 결과 
  - Topic_importance.xlsx: 각 Topic의 Stock을 계산하여 Topic별 중요도 산출 결과
  - Topic_satisfaction.xlsx: 각 Topic에 속하는 키워드와, 키워드들의 평균 감성점수를 이용하여 Topic별 만족도 산출 결과
  - Opportunity.xlsx: Opportunity algorithm을 이용하여 최종 토픽별 기회수준 분석 결과