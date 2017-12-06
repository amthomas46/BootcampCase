# Bootcamp Case

## Scenario
You've been assigned a new customer, Contoso LLC, which sells bicycles and bicycle equipment to its customers. Contoso currently processes new product orders and queries through human operators. They are looking for an automated solution that allows Contoso to seamlessly scale up to handle large call volumes while maintaining zero wait times and freeing up staff to manage other tasks. Currently, their product inventory is stored in Azure SQL.

## Architecture
Your team recently presented a potential architecture (below) that Contoso LLC approved. 

![architecture](/images/arch.png)

* [Skype Client](https://www.skype.com/)  
User initiates call
* [Bot Connector](https://dev.botframework.com/) + [Skype Calling Channel](https://dev.skype.com/bots)   
Routes calls from Skype to the bot
* [Azure App Services](https://docs.microsoft.com/en-us/azure/app-service/)  
Hosts the bot application, which manages logic and API calls
* [Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/)  
Stores bot state and event logs
* [Bing Speech Service](https://docs.microsoft.com/en-us/azure/cognitive-services/speech/home)    
Processes speech-to-text
* [LUIS](https://docs.microsoft.com/en-us/azure/cognitive-services/LUIS/Home)  (Language Understanding Intelligent Service)  
Extracts intent and entities from text
* [Azure Search](https://docs.microsoft.com/en-us/azure/search/)  
Indexes the product catalog for product-query matching
* [Azure SQL](https://docs.microsoft.com/en-us/azure/sql-database/)  
Stores product and order data
* [Azure Storage](https://docs.microsoft.com/en-us/azure/storage/)  
Stores bot audio data for debugging

## Day 1 Assignment
Your team is preparing a proof of concept, and your group has been tasked to suggest answers to the following questions:

1. Which features from Azure Search should you take advantage of?  
2. What might your main intents in LUIS be?  
3. What are some tasks you'll have to complete to create an efficient and functional calling bot? (e.g. incorporating the LUIS model, enabling your bot to speak)  
4. Are there any additional Cognitive Services that you think the bot would benefit from?  

Document your suggestions on the whiteboards/flipcharts provided. You will present your results.