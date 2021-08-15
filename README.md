# glg-fourthbrain

Create an expert recommendation system based on previous requests by clustering them using the LDA algorithm. 

The new request experts are recommended once a table is created that summarises the main topics and experts in those fields.

| Topic_id | Topic_terms                       | Experts      |
|----------|-----------------------------------|--------------|
| 0        | facebook, user, app, social_media | name1, name2 |
| 1        | health, medical, patient          | name0, name3 |
| ...      | ...                               | ...          |

Each document has topics related to it and a percentage of contribution by each topic. 

Once a request is received it is embedded using the universal sentence encoder and the distance is calculated with the ones of the previous documents and the top k related documents, terms and experts are printed. 

