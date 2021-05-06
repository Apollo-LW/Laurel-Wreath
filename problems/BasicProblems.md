# Objects
- Too heavy, and most of the data that are returned is not used. Which affect both our Kafka Streaming and our latency in the REST API that the microservice provides.
- Identical, objects aren't compared by ID, which they must be to solve the redundancy problem, as well as the delete operations
- Objects that are send with the request should also be light, as well as have constant fields so they don't change in anyway.
- Wrapper classes vs primitive data types

# Security
- There is no security implemented what so ever, no authentication, no authorization, no accounting [ZERO](https://64.media.tumblr.com/e9f5a52f4563ee58a151e0f98d6d36b4/tumblr_pvcwrrtu7K1xpdwtoo1_540.gifv), not in the gateway, not on certain objects, not on any API.

# Real Time
- Real time is present in some places that doesn't need "real time", which affect APIs and streaming overhead. As well as, some enities are not updated in real time in the kafka cluster.

# Documentation
- Documentation is poor in most of our microservices, which results in poor maintainability 

# Search Engine
- Don't even get me started. We have an awesome search engine, but it lacks reliablity and preformacce, as well as language training is not preserved, which is basically a fibonacci sequence recursion function without it's memoization table (computing many things over and over again althought it seen it before).
- It also can be imporved in begin more "smart", especially in arabic, where we provide translation for data to be able to search any data in any language.

# API
- Error Handling, errors can literally bring our whole stack down like it's nothing, so we need to prevent them.

# Abstraction
- Data Structures used in models are not that abstract, which leads to poor encapsolation, thus poor API interface.

# Easter Eggs
- There should be easter eggs for testing purposes, this is not a problem, this is just a good way to test how well our microservices are doing.

# Naming Conventions
- We should follow a more strict naming convention, to provide maintainability and to understatnd things better (code readability)

# Unnessary Files and Scripts
- Overhead, the more files we have the more overhead we'll create for the API and same goes in the front-end