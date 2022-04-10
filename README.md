# NLP_robo_advisor
nlp robo advisor for digital transformation consultant
# Project usage
In this project I created a NLP bot for a prominent retirement plan providers.
## Instructions
This section divides the Challenge instructions into the following three steps:
-Configure the initial robo advisor

-Build and test the robo advisor

-Enhance the robo advisor with an Amazon Lambda function

### Step 1: Configure the Initial Robo Advisor
In this section we configured the bot, by setting up the criteria for the bot including:
-language
-session timeout
-output voice
-Bot Name
-Intent slots
-Confirmation slots
-sample utternaces which include:
--I want to save money for my retirement
--I'm {age} and I would like to invest for my retirement
--I'm ​{age} and I want to invest for my retirement
--I want the best option to invest for my retirement
--I'm worried about my retirement
--I want to invest for my retirement
--I would like to invest for my retirement
### Step 2: Build and Test the Robo Advisor
In this section we built the bot and tested the core functions to ensure the bot was working.
The test_nlp_bot_works.png is a picture that shows the bot works.
### Step 3: Enhance the Robo Advisor with an Amazon Lambda Function
In this section we did the following objectives and the test objectives are shown in the attached png files:
-Create a new Lambda function from scratch, and name it recommendPortfolio. Choose Python 3.7 as the runtime programming language.
-Complete the recommend_portfolio function by adding the following validation rules:
--The value of age should be greater than zero and less than 65.
--The value of investment_amount should be greater than or equal to 5000.
-Complete the starter code so that once the intent is fulfilled, the bot responds with an investment recommendation based on the selected risk level, as follows:
--None: “100% bonds (AGG), 0% equities (SPY)”
--Low: “60% bonds (AGG), 40% equities (SPY)”
--Medium: “40% bonds (AGG), 60% equities (SPY)”
--High: “20% bonds (AGG), 80% equities (SPY)”
-When you finish coding your Lambda function, test it by using the provided test events.
-After successfully testing your code, open the Amazon Lex console, and then navigate to the recommendPortfolio bot configuration. Integrate your new Lambda function into the bot by selecting it in the “Lambda initialization and validation” and “Fulfillment” sections.