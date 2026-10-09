# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?

 At first glance, I noticed that the attempts on the left side didn't match up with the attempts on the right side. 

- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

  1. There is no "8" attempts, only allows 7. Expected to have all 8 attempts, not 7. 
  2. Hints are backwards. Example, when guess is 67, I input 40 and the hint says to go higher. 

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|guess of 40|"Too Low" hint | "Too high" shown| Console Output :None                   |
|start new game| give a new secret number| does not start a new game| Console Output: None|
|last attempt not the secret number |Lose game, play again|Lost game could play agian |Console Output: None |

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?

Claude

- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).

One example is Claude Ai suggested that lines 31-48 mesages needed to be swapped. 

- Give one example of an AI suggestion you did not accept as written (including what the AI suggested, why you rejected or changed it, and how you verified your version). It does not have to be a suggestion that was wrong: over-engineered, out of scope, harder to read, or a poor fit for this codebase all count.

At first, when I pasted the app.py code into the app, Claude claimed there were no errors. I knew there was an error to fix. I believe it may have been confused by the wording of my question. 
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?

I decided a bug was fixed by testing after very edit to make sure what needed to be fixed was fixed. 

- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.

  I ran a manual test when checking to see if the bugs. It showed me that the code needed to be edited in some places.

- Did AI help you design or understand any tests? How?

Ai did not help me desgin or undersatnd any tests. 


---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

It's a tool that makes it much less complicated to build an app. It's basically like a brain connecting memories and remembering things. 

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.

The strategy of marking the places that are not working the way I want it to.

- What is one thing you would do differently next time you work with AI on a coding task?

Make more clear instructions. When asking ot do something i need to state waht I need more clearly. 

- In one or two sentences, describe how this project changed the way you think about AI generated code.

This did not change much of how I think about AI-generated code. I already knew it wasit wasn't fully reliable and neededneeded to be checked. 
