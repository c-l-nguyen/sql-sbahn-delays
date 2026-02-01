# sql-sbahn-delays
Exploring DuckDB and SQL techniques using Berlin S-Bahn delay dataset. This dataset comes from a sample dataset from [Kaggle](https://www.kaggle.com/datasets/alperenmyung/berlin-s-bahn-punctuality-database/data) called "Berlin S-Bahn Dataset" which contains data about Berlin S-Bahn trips, delays, and events like strikes, incidents, events, and weather. The data is downloaded as a SQLite relational database but I load it into DuckDB just to test DuckDB. It's not a very large dataset to need to use an OLAP database like DuckDB but I just want to test its capabilities.

Sample questions you can ask about this data (that I would ask in a theoretical SQL interview):

1. Which lines are the most frequently delayed? What can you tell me about delays using only the `trips` table? What about cancelations?
2. Combine the `trips` table with one or more other tables. What patterns in the delays do you see and can you show me how you came to your conclusions?
3. It is said that "the 4 biggest enemies of Deutsche Bahn are the Spring, the Summer, the Fall, and the Winter" (original: Die vier größten Feinde der Deutschen Bahn: 1. Frühling 2. Sommer 3. Herbst 4. Winter). Incorporate the `weather` table into your analysis. What can you say about how weather affects delays and cancelations?
