## Chat with your data stored in Astra DB, DataStax Enterprise or AstraDB using an LLM

This code provides a demonstration of a Natural Language Interface to Data. It leverages DataStax Enterprise v7 or Apache Cassandra as the database, Ollama as a local inferencer, and LLama2 as the LLM. 

The system allows users to ask natural language questions about their data stored in DataStax Enterprise or Cassandra. The application converts the natural language questions into CQL queries, executes them against the database, and provides a user-friendly natural language response.

### Inputs

The application accepts natural language questions from the user. For example:

* "Where did I purchase coffee?"
* "How many coffees did I purchase in March 2023? My credit card number is 1234567890123456"
* "What's the total amount of money I spent in March 2023? My credit card number is 1234567890123456"

### Outputs

The application returns a natural language response to the user's question based on the results of the CQL query executed against the database. For example:

* **User Question:** "Where did I purchase coffee?"

    **Answer:** 
    "Oh, wow! Based on the results from your query, it looks like you purchased coffee at two different locations! 😃

    The first transaction occurred at a place called "Coffee Shop" and the second one was at another coffee shop called "Morning coffee". 🎉

    So, to answer your question, you purchased coffee at both of these places using your credit card number 1234567890123456! 😊"

* **User Question:** "How many coffees did I purchase in March 2023? My credit card number is 1234567890123456"

   **Answer:** 
   "You purchased 2 coffees in March 2023."

* **User Question:** "What's the total amount of money I spent in March 2023? My credit card number is 1234567890123456"

   **Answer:** 
    "The total amount of money you spent in March 2023 is $480.74."
