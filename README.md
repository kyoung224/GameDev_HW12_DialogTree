# GameDev_HW12_DialogTree

Starting code given by professor, Michael Weeks.

## Directions: https://hallertau.cs.gsu.edu/~mweeks/csc4821/HW12.html

Your book Fundamentals of Game Design, third edition (by Ernest Adams) presents dialog trees as a way to handle scripted conversations. Start by refering to figure 11.5 in your textbook. For this assignment, you are to implement the conversation from "Ask about evidence" on down.

There is an example program at https://gamedev.cs.gsu.edu/~mweeks/dialog_tree_v2.html. It presents a prompt, "Select your response", along with several options such as "yes", "maybe", and "no". Each option has a letter next to it. When you choose a response, the system processes it. You should observe two things: the "no" and "maybe" responses disappear from the menu when selected, and that there is some feedback at the bottom under "Results:". This program demonstrates the idea of a dialog system. You can use this as a starting point to implement your solution.

In the book's figure 11.5, there are options on the left corresponding to the choices to present to the player. For example, the "Ask about evidence" options should be "Did you hear any shots around that time?", "We're trying to trace a tall man in jogging clothes. Did you see him?", "When you came out, did you see a blue car go by?", and "That's all we want to know for now." When the player chooses one of these options, respond with the text on the right. For example, choosing the first option should result in a response of "No, no shots. I'd remember shots". Both the selected text and the response should appear in the "Results" section. This will keep a log of the interactions. Following the arrow on the right (next to "No, no shots. I'd remember shots"), we see that it points back to this part of the conversation (also called "prompt and options set" below). In that case, remove "Did you hear any shots around that time?" from the options.

In the case that it reaches an "end", turn the background to a noticably different color (such as green), and do not process any more input. Add the word "end" to the Results.

In the case that the arrow leads to another prompt and options set, such as "About the car", be sure to remove all unused options, add the new options, and change the text accordingly.

It's possible that the arrow leads to a different prompt and options set, but one that has already been shown. In that case show it just like you did the first time, i.e. with all of the options.

Your completed solution should implement the conversation from "Ask about evidence", on down, from Figure 11.5. Note that one of the arrows in the "follow-up" menu points back to the menu above "ask about evidence". In this case, have it point to "ask about evidence" instead.

Feel free to make improvements.

Turn this in through iCollege: a link to the html file, copies of any javascript files that you created, and any data files.
