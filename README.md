# Service Quality and Customer Satisfaction: Text Mining of Online Hotel Reviews
In this project, we have extracted the data from tripadvisor.com. The data has 15,493 online reviews on 27 hotels written between 2010 and 2023 which can separate into
- 1,354 reviews on 2-star hotels
- 3,745 reviews on 3-star hotels
- 4,885 reviews on 4-star hotels
- 5,509 reviews on 5-star hotels

The dataset has the customer satisfaction score of the reviewers measured on a scale ranging from one to five and it also had textual reviews written in the English language. 

Therefore, this project will use text-mining techniques to measure the service quality (SERVQUAL) dimensions and their impact on customer satisfaction based on customers’ reviews by using two attributes from the dataset which are customer reviews to find the service quality (SERVQUAL) dimensions and the rating from customers referred to their satisfaction. 

### Service Quality (SERVQUAL)
The service quality (SERVQUAL) model focuses on the gap between the expectations of the customer before receiving and their perceptions of the actual service delivered. The five dimensions of service quality (SERVQUAL) model represent in this paper are as the following:
- Tangibility: the impression of the physical facility, personnel, communication materials on the buyer and equipment
- Reliability: accuracy of the service
- Responsiveness: willingness to provide prompt service and quick response to customer questions or complaints
- Assurance: the knowledge and behavior of workers which generates trust and credibility for customers
- Empathy: provision of care, and individualized attention that the organization provides to its buyers

Before analyzing data, we have done the pre-processing data and transformed data into the proper form to analyze by using Microsoft Excel. We have gathered data from each hotel following the hotel star ratings which are an internationally- accepted indicator of a hotel’s quality, cleanliness, and standards. The hotel star rating helps customers understand the quality of the hotel which also makes it easier for customers to compare hotels and make booking decisions and understand what they could reasonably expect when staying at a hotel which leads to customer satisfaction. In this research paper, the star rating is classified according to Giata [29]. After that, we have randomly selected 300 reviews from each hotel star rating to eliminate the bias from hotels in that hotel class to be the representative of each hotel rating class. The 300 reviews are divided into 3 categories which are as the following:
- The reviews which a rating score from customers equal to 4 to 5 as positive reviews to represent customer satisfaction 100 reviews: the customers are satisfied with the hotel
- The reviews which a rating score from customers equal to 3 as neutral reviews to represent customer neutral 100 reviews: the hotel is equal to the customer expectations.
- The reviews which a rating score from customers equal to 1 to 2 as negative reviews to represent customer satisfaction 100 reviews: the customers are dissatisfied with the hotel

### Method
1. Extract the customer reviews from the online platform
2. Do the preprocessing and transform data into the proper form to analyze
3. Identify the SERVQUAL dimensions by using zero-shot classification: the facebook/bart-large-mnli model as a single class classification
4. Analyze the relationship between service quality and customer satisfaction by hotel classes
