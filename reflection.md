# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?

The game look okay because I could see the title and where to input a guess

- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

The hint were wrong, the game would suggest to go lower while going higer was the right choice and vice versa
The game difficulty was also wrong and matched incorrectly (hard wasnt actually hard, easy wasnt actually easy)
The range input wasnt updates as the game difficulty mentioned. the input was always 1 to 100. 

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?

Claude and Copilot

- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).

The AI suggestion for changing the if conditions output when the guess is compared to secrete was correct. This was verified form the app UI when i plugged in a number the correct hint out put was given compared to the input guess. 

- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

No AI suggestion that i rejected the suggestions looked good so I approved them and tested then by running the game and pytest
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?

By running the app and trying different inputs to verify.

- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.

  By selecting the mode manually from the app, it showed an updated matching that is correct:

  The hard guess range was the biggest, then the medium and then the easy. This made me confirm that the part of the code was now working


- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

I would simply say streamlit reruns the entire script on every interactions and prevents the data from being reset between those reruns. 

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?

The testing habit

  - This could be a testing habit, a prompting strategy, or a way you used Git.


- What is one thing you would do differently next time you work with AI on a coding task?

First try to write down all the bugs I noticed in a very simple way, before AI assistance

- In one or two sentences, describe how this project changed the way you think about AI generated code.

This project was really go and it changed the way I think about AI generated code. This is because this code
is not always right and can contain many bugs. So the power is in the testing and improving the code and using AI as an assitant that you have to
check what they did always. But coding with AI is certainly much easier. 
