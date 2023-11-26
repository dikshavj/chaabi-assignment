# Chaabi_assignment

## Overview of the model:
- Used Qdrant Vector base to store the embeddings of given data
- Concatenated product name, category, sub category, brand and description data of each product into vectors
- Implemented BERT LLM model on the top matched products obtained from similarity search from vector base to get output
- Wrapped the model as an REST API using Flask 


## Sample Queries:

1. question = "which product is produced by Nutrashil brand"
  - Answer:  Nutriorg Jamun Honey 
  - Title:  Certified Organic Jamun Honey 
  - score:  0.7772384881973267

2. question = "Which product contains garlic oil"
  - Answer:  Colavita Extra Virgin Olive Oil 
  - Title:  Garlicolio - Garlic Seasoning Made With Extra Virgin Olive Oil 
  - score:  0.5382457971572876

3. question = "What is called as Indian superfruit and also an Indian gooseberry?"
  - Answer:  amla 
  - Title:  Amla 
  - score:  0.9943625330924988

4. question = "What wax is a sculpting product in the Schwarzkopf line? "
  - Answer:  Taft Hair Wax 
  - Title:  Taft Shine Gel Wax 
  - score:  0.8936730027198792

5. question = "What is the size of designer glass bowl? "
  - Answer:  280 ML 
  - Title:  Designer Glass Bowl 
  - score:  0.7578027248382568

