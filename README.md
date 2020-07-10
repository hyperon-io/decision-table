This repo is prepared to demonstrate how to execute decision table using [Hyperon.io](https://www.hyperon.io).

# What is decision table? 

Decision table is one of the ways of implementing business rules in IT system. It describes what decisions should be made given input values. In Hyperon decision table is called parameter and input values are organized as input levels. Decision to be made is output level. 

From user perspective decision table is very similar to Excel sheet, but instead of enumerating all values you can make it in more clever way: as range, from - to, as "*" meaning all values or... as other parameter/decision table. Yes, you can stack them to create more complex decisions! 

More on the decision tables with examples you can find in this [article](https://www.hyperon.io/usecase/business-rules-management-system) and in Hyperon [documentation](https://www.hyperon.io/tutorial/hyperon-concepts-parameters)

# How to execute decision table? 

There are three ways to do so: 

## Using REST interface 

Just provide all your context (key - value pairs) of business data needed to make decision and list of decision tables to evaluate (parameters). 

Documentation for this interface: [REST API - execution](https://www.hyperon.io/docs/rest-api#execution) 

## Using Java Hyperon Runtime Component

Same as above but in Java :) 
Main advantage of using Java library is performance! Although REST API have in memory caches implemented there is always small fraction of time needed to initiate HTTP connection. With java library you don't have dease overhead - and have all the caching. 

How to for this interface [Programming with Hyperon tutorial](https://www.hyperon.io/docs/programming)

## Using tester in Hyperon Studio 

Final and quickest method do call decision table is by using buit-in tester in Hyperon Studio. 
It's best option for testing newly created decision tables. Hyperon will ask you to provide all business data needed to make decision. 

More in Hyperon[User Guide](https://www.hyperon.io/docs/guide/simulations#tester)


Example code is coming soon. 
