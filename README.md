# Digital Psychotherapist - Chatbot on Python from Scratch using Regex

This program is a designed chatbot that will have a dialogue with the user based on the inputs it receives from the user. Similar to 
Joseph Weizenbaum's Eliza, the purpose of this chatbot is to be able to act as a digital psychotherapist. The goal of this project was to model 
Weizenbaum's work from 1964 - it is a rather simplistic chatbot. 

Our program recognizes the specific 
keywords and based on the user's input, it analyzes the sentiment of the input and responds accordingly. We also designed a GUI for our program 
for a better user experience (additional functionality of the program which still we are working on it to develop it more). Once you run the code, 
the program initiates a dialogue by asking the user’s name and then the conversation continuous based on the user’s next input.

Below is sample ELIZA dialogue window.

[ELIZA]: Hi, I am Eliza, your digital psychotherapist. I can help you with whatever's bothering you.

[ELIZA]: At any time you can close this session by saying "quit"

[ELIZA]: Let's start. What is your name?

[You: ] John Doe

[ELIZA]: Hi John, how can I help you today?

[You: ] I feel sad.

[ELIZA]: I'm sorry to hear that. Why do you feel sad?

[You: ] I don't know.

[ELIZA]: It's okay to not know everything today, learning is a proccess.

[ELIZA]: Would you like to share more about it?

[You: ] I think about suicide.,

[ELIZA]: Help is available, speak with someone today. 
988 Suicide and Crisis Lifeline 
Hours: Available 24 hours. 
Languages: English, Spanish.

[ELIZA]: Tell me why you feel that way.

[You: ] kdkbkbie

My linguistic skills are not as refined as the human beings I immitate. Could you please help me understand you what mean? .........

Algortihgm Description:

The algorithm takes a series of inputs from the user and returns an output in a manner imitating a psychotherapist. Regex is used to process the inputs provided by the user. The algorithm begins by asking for the user’s name and this name is later used to tailor the conversation with the user, such that the program refers to the user by their name. Moving forward, the program asks the user how it can help them and chooses a function to generate a response depending on the user’s response. These functions have been designed to handle statements depending on whether they start with ‘I feel like…’, ‘I need….’, ‘I want….’ Etc. A sentiment analyzer has been installed to run an analysis on every statement provided by the user, this helps the program respond accordingly (depending on whether the user is in a positive or a negative mood). Moreover, a filler function has been implemented that handles all other statements from the user that the program is not programmed to handle in a customized manner. The program also runs a check on each statement to understand if there is any mention of ‘suicide’, in which case the program uses Google’s suicide prevention response. The algorithm has been designed to be logically robust against a variety of statements.

Extra Functionality:

Tailoring responses depending on the sentiments of the user.

Suicide prevention mechanism which is triggered from any mention of the word suicide.
