Lists 
======

.. include:: blocks.txt

.. include:: icons.txt

.. infonote::

 |intro9s|

In the programs we created in the previous lessons, we used only simple data types - each variable kept the value of one piece of data. However, we often need to store a whole set of data under one name, for example, a set of numbers. If we want to store phone numbers of 10 of our friends, we will need to create 10 variables, which is not easy to maintain, so we will use a complex data type, which in Scratch is called a **list**.

.. infonote::

 **What is a list?**

 A list is a complex variable that is made up of multiple elements - multiple variables. These can be different types of data; in this example they are strings. It is created similarly to how ordinary variables are created.
   
 (1) In the group *Variables* click on the button *Make a List*. 

 (2) A dialogue window will appear where you should write the name of the list and confirm by clicking the *OK* button. 

 .. image:: ../_images/9/fig9_1.png
     :width: 575px   
     :align: center

 (3) A blank monitor of the list will appear on the stage, and the bottom of this monitor will have the current length of the list written on it, which will be 0.
   
 (4) Clicking on the sign "+", located in the bottom right corner, will open the field where you can enter your first element, and the length of the list will increase by 1. 

 (5) The first element of the list should be entered in the blank field.

 .. image:: ../_images/9/fig9_2.png
     :width: 370px   
     :align: center
   
 By repeating this process, the desired number of list elements can be entered.

 At the same time, a block associated with the list and 11 other blocks that allow the list and its elements to be used in the program, will appear in the block palette.

 .. image:: ../_images/9/fig9_3.png
     :width: 420px   
     :align: center



|study| Study the following examples
----------------------------------------

In the project called "Quiz", there is a list of questions and a list of correct answers. Questions and answers can be entered in advance, or they can be uploaded from a text database. The program asks the questions randomly and then checks if the answer given by the user is correct. If the answer is correct, the user will receive a point, and if not, the program will broadcast the correct answer. In the end, based on the number of correct answers, the user receives a grade.

Example 1 - Project "Quiz"
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

In this example, we will illustrate how a math quiz can be made. The quiz checks if participants are able to determine the greatest common divisor for two or three numbers.
The questions are located in the list *Numbers*, and the answers in the list *GCD* (greatest common divisor). We will use the variable **k** to go through the lists, the value of this variable changes from 1 to 8 (the number of list elements), and we will store the number of correct answers in the variable **b**.

.. image:: ../_images/9/fig9_4.png
     :width: 440px   
     :align: center

The script for this project can be seen below.

.. image:: ../_images/9/fig9_5.png
     :width: 565px   
     :align: center

The following project illustrates how the list elements can be selected randomly. We will use the reporter block, which will return the value of the list element whose sequence number is written in the appropriate input field. This way, if we randomly generate the variable *number*, by entering that number into the sequence number input field, we will get the element, which is in that position on the list. The project also illustrates how randomly generated numbers can be used for broadcasting different messages.

.......

Example 2 - Project "Hunger"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

There are 10 sprites participating in this project - hungry cat and 9 types of food the cat is fantasizing about. 

.. image:: ../_images/9/fig9_6.png
     :width: 460px   
     :align: center

The cat is walking left and right, and "thinking" for 3 seconds one of the 11 sentences, chosen randomly, from the list of sentences called *food*. 

.. image:: ../_images/9/fig9_7.png
     :width: 220px   
     :align: center

During the time the cloud is visible on the stage |think_sec|, the image of the food the cat is thinking about appears in the white cloud located in the center of the stage.

.. image:: ../_images/9/fig9_8.png
     :width: 960px   
     :align: center

The synchronization of the appearance of the food and cat's thinking about that particular food will be achieved with the broadcasting of messages. 

The variable *number*, which is generated randomly is used both for selecting the sentence from the list *food* and for generating the message from "1" to "11". No one reacts to the messages "1" and "11", while sprites whose names are numbers between 2 and 9 will react to the messages from "2" to "9". 

For example, the mouse who is sprite "2" will react to message "2", the bird who is sprite "3", will react to message "3", etc.

.. image:: ../_images/9/fig9_9.png
     :width: 660px   
     :align: center

The reaction of each sprite is the same: they appear for 2 seconds, while the cat's thinking cloud is visible, and then they hide again. When the green flag is clicked, all sprites (except for the cat) go to the position (0,110), which is the center of the white cloud, and they hide.    

The following figure contains all scripts added to the main sprite of this project. 

.. image:: ../_images/9/fig9_10.png
     :width: 385px   
     :align: center

.......

The following project illustrates how we can divide all objects into groups of desirable, undesirable and neutral. The record of desirable objects is stored in one list, and of undesirable objects in another list. When the object is chosen, the program first checks to which group it belongs: if it is desirable, positive points will be obtained, and if it is undesirable then negative points will be obtained; if it is neutral, the number of points will not change. For example, this could be the strategy if you are making a game for kids, where they need to collect as many useful items as possible and avoid dangerous items (see project tasks).

Example 3 - Project "Food"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

**The scenario of the project**

The main sprite of this project is a girl called Zara. During school recess, she can eat something, drink water or take a gift. You choose what Zara will take by clicking on the objects that appear on the stage. If you choose fattening food - a sandwich, chips or a donut, you will receive negative points. If instead you choose fruit - an orange, a banana or an apple, you will receive positive points. If you choose to get water or the gift, the points will remain unchanged.  

.. image:: ../_images/9/fig9_11.png
     :width: 400px   
     :align: center

The names of items that earn positive points are in one list (in our case "fruit"), and those that earn negative points in the other (in our case "unhealthy"). 

**Behavior of the sprites**

All items have the same behavior. When the green flag is clicked, they appear on the randomly chosen position on the right side of the stage. When the user clicks on them, they assign their name to the variable *food*, broadcast the message *taken* and hide. 

.. image:: ../_images/9/fig9_12.png
     :width: 815px   
     :align: center

The scripts added to Zara also allow the program to calculate the number of points depending on which food was selected. 

.. image:: ../_images/9/fig9_13.png
     :width: 495px   
     :align: center

.......

Example 4 - Project "Clumsy Wizard"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 3

The main sprite of this game is the Clumsy Wizard. He can use his magic wand to make multiple copies of the same thing, but he often gets confused and forgets exactly how much he promised, so he makes too many items or not enough.

There is also his assistant, Wizard Girl, who keeps a close eye on what Clumsy Wizard has promised and how many copies he has made, reminding him if he makes a mistake.

.. image:: ../_images/9/fig9_14.png
     :width: 600px   
     :align: center

**How the Clumsy Wizard promises different things**

To allow the Clumsy Wizard to promise to make different things, we need to create a sprite with those things as its costumes. Apart from that, we need to make a list with the names of those things. In our project, we will create a sprite called the *Creature*, which can appear in 5 different costumes. 

.. image:: ../_images/9/fig9_15.png
     :width: 630px   
     :align: center

In order for the Clumsy Wizard to be able to say the names of the costumes, we have introduced a list called *things* and into it, we entered 5 costume names. A number between 1 and 5 is randomly generated and then the Clumsy Wizard says a sentence in which the text "Now I will make" is joined with the corresponding element from this list. For example, if number 2 is generated, the Clumsy Wizard will say "Now I will make apples", and if number 4 is generated, he will say "Now I will make butterflies".

The following figure shows the behavior of the wizard sprite when the user clicks on him. First, the value of the variable *number* will be randomly generated from the interval [1,5]. Then, the wizard says that he will make one of the costumes of the sprite *Creature*, more specifically the one whose sequence number in the list is the same as the generated number. Then, he broadcasts the message *Show off* to which the Wizard Girl will react by asking the Clumsy Wizard how many copies of the creature he intends to make, her question will last for 2 seconds. This is why there is a block added to the wizard, which allows him to wait for 2 seconds. After this pause, the wizard will generate the value of the variable *how* from the interval [1,10]. 
Since the costume dimensions of the sprite *Creature* are set to about 50x50 pixels, we decided that the maximum number of creatures that can be "created" by the Clumsy Wizard should be 10. This way, all of the copies will be visible on the stage. The Clumsy Wizard says how many copies he will create and broadcasts the message *create*.

.. image:: ../_images/9/fig9_16.png
     :width: 460px   
     :align: center

The following figure represents the scripts, which describe the behavior of the Wizard Girl. She reacts to both messages broadcast by the wizard, and she broadcasts her own message *hide* 4 seconds after she has received the message *create*. The message *hide* is the signal for the creature sprite to remove its clones and itself from the stage. 

.. image:: ../_images/9/fig9_17.png
     :width: 490px   
     :align: center

The following figure represents the scripts, which describe the behavior of the *Creature* sprite. This sprite reacts to 4 different events: clicking on the green flag, broadcasting the messages *create* and *hide*, and the cloning event. When the green flag is clicked, the creature hides, and when it receives the message *hide*, it changes the value of the variable *next*. This variable, unlike the global variables *number* and *how*, which can be used by all sprites, is created only to be used by the *Creature* sprite, so it is a local variable. The main characteristic of local variables is that they can be used only by the sprite they were created for. Other sprites can see their values, but they cannot change them. The variable *next* is used as a trigger. When its value changes from 0 (initial value that is set at the beginning of the reaction to the message *create*) to 1, the destruction of the clones (copies) begins, and the sprite hides. 

.. image:: ../_images/9/fig9_18.png
     :width: 170px   
     :align: center

**How does the Clumsy Wizard display the different number of sprite's copies (clones)?**

One more thing we need to explain is how the Clumsy Wizard is able to display multiple copies of a certain sprite (i.e. of costumes of the *Creature* sprite). For this, he uses the **cloning** of sprites. We have shown already that the sprite (and all scripts added to it) can be multiplied during the creation of the program. The multiplication is done by selecting the option *duplicate* from the shortcut menu that you get when you right-click on the sprite in the sprites list. In Scratch, there is also the option that allows the sprite to be multiplied during the running of the program. (It is similar to lists, to which the elements can be added both during the creation and running of the program) 

To clone the sprite and to manage the behavior of the clone, we use the instructions |create_clone| and |when_clone| from the group *Control*. In the script describing the behavior of the creature sprite when it receives wizard's message *create*, the sprite appears on the left edge of the stage, after which its clones are created and displayed on the stage. Each clone is displayed at a distance of 50 steps from the previous one, so they stand side by side in a row. This is achieved with the loop that is repeated *how-1* number of times, which, together with the original sprite, produces the promised number sprite copies. Since the variable *next* is a local variable for the sprite that is being cloned, each of its clones has its own value of this variable, and all of the clones are visible on the stage until the variable *next* receives the value 1 (when the sprite receives the message *hide*). This is when each clone deletes itself, and the original sprite hides. 

.. image:: ../_images/9/fig9_19.png
     :width: 430px   
     :align: center

**Upgrading the project Clumsy Wizard2**

The idea of this upgrade is to arrange so that the wizard does not make as many copies of the object as he promised. He makes either too many or not enough. The user should say how many more or fewer objects the wizard has created, i.e. the child should learn to add and subtract numbers up to 10. We achieve this by generating the variable *error*, whose values can be integer numbers from the interval [-3,3]. Of course, if the generated error is 0, the wizard will create the exact number of copies he promised, but in other cases it will be necessary to determine how many objects he has created. The following figure shows some of the cases when the wizard gets "confused". 

.. image:: ../_images/9/fig9_20.png
     :width: 610px   
     :align: center

The following script describes the behavior of the creature.

.. image:: ../_images/9/fig9_21.png
     :width: 410px   
     :align: center

The script presented below describes the behavior of the Wizard Girl.

.. image:: ../_images/9/fig9_22.png
     :width: 550px   
     :align: center

Save this modified project under the name *Clumsy Wizard2*. 

Note. If the project is used to practice adding and subtracting with numbers up to 10, it will be useful to insert a "blank" question |ask_wait| into the script added to the young girl wizard instead of the wait block |wait_sec|. Only when the child gives the answer, will we press *Enter* and check that answer. 

|ask| Answer the following questions
--------------------------------------

For all the questions that follow, it is assumed that, initially, the list has the following elements

.. image:: ../_images/9/q9_1.png
     :width: 125px   
     :align: center

Question 1
~~~~~~~~~~~

.. level:: 1

.. mchoice:: lista1
   :multiple_answers:
   :answer_a: the list will have one less element 
   :answer_b: the element orange is in the number 1 spot on the list
   :answer_c: the element is moved to the end of the list
   :answer_d: the last element on the list is taken out
   :correct: a, b
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   What is the result of the execution of the command |l1|? (Select all correct answers) 

.. |l1| image:: ../_images/9/l1.png
  
Question 2
~~~~~~~~~~~

.. level:: 1

.. mchoice:: lista2
   :answer_a: the element will be added to the beginning of the list 
   :answer_b: the element will be added to the end of the list
   :answer_c: the element will be added under the condition it was not previously on the list
   :correct: b
   :feedback_a: This command adds to the end of the list.
   :feedback_b: Correct.
   :feedback_c: No checks are made.
   
   What is the result of the execution of the command |l2|?

.. |l2| image:: ../_images/9/l2.png

Question 3
~~~~~~~~~~~

.. level:: 1

.. mchoice:: lista3
   :answer_a: zero
   :answer_b: one time
   :answer_c: two times
   :answer_d: three times
   :correct: d
   :feedback_a: The list has 3 elements. 
   :feedback_b: The list has 3 elements.
   :feedback_c: The list has 3 elements.
   :feedback_d: Correct.

   How many times will the sprite says "I like fruit"?

   .. image:: ../_images/9/q9_3.png
      :width: 220px   
      :align: center

Question 4
~~~~~~~~~~~

.. level:: 2

.. mchoice:: lista4
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :correct: b, c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   
   Which command will place the element *strawberry* in the second position in the list *fruit*? (Select all correct answers) 

   .. image:: ../_images/9/q9_4.png
      :width: 650px   
      :align: center

Question 5
~~~~~~~~~~~

.. level:: 2

.. mchoice:: lista5
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :correct: a, b
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   
   After the execution of which commands will the number of elements in the list increase? (Select all correct answers) 

   .. image:: ../_images/9/q9_4.png
      :width: 650px   
      :align: center

Question 6
~~~~~~~~~~~

.. level:: 2

.. mchoice:: lista6
   :answer_a: If the list includes the element strawberry, its size will not change; otherwise, the element strawberry will be added to the end of the list.
   :answer_b: Regardless of whether or not the element strawberry was included, it will add it to the end of the list.
   :answer_c:If the list includes the element strawberry, its size will not change; otherwise, the element strawberry will be added to the beginning of the list.
   :correct: a
   :feedback_a: Correct.
   :feedback_b: List entry is accomplished if the list did not previously have the element strawberry.
   :feedback_c: If it is added, it will be added to the end of the list.
   
   What is the result of the execution of the following commands?

   .. image:: ../_images/9/q9_6.png
      :width: 300px   
      :align: center

|try| Try it!
--------------

In the first 3 exercises, it is assumed that we have a list called **original**, whose elements are numbers from 1 to 10 (in sequence).

Exercise 1
~~~~~~~~~~~
.. level:: 2

.. infonote::

  Write a script, which creates the list called **duplicate** and writes into it all the elements of the existing **original** list.

.......

Exercise 2
~~~~~~~~~~
.. level:: 2

.. infonote::

  Write a script that creates a list called **backward** and writes into it all the elements of the existing list **original** in the reverse order, i.e. the first element of the list *backward* should be the last element of the list *original*, the second - the penultimate from the list *original* and so on until the first element of the list *original*, which should be the last in the list *backward*. 

.......

Exercise 3
~~~~~~~~~~
.. level:: 2

.. infonote::

  Write a script that creates the list **even** and writes into it every other element of the existing list **original**.

.......

Exercise 4
~~~~~~~~~~~
.. level:: 2

.. infonote::

  Write a script that creates the list **random1** and writes into it 10 numbers from the interval [1,100], generated with the operator random number.

.......

Exercise 5
~~~~~~~~~~
.. level:: 3

.. infonote::

  Write a script that creates the list **random2** and writes into it 10 DIFFERENT numbers from the interval [1,100], generated with the operator random number.


|bug| Debug it!
----------------

Bug 1
~~~~~~~~

.. level:: 2

.. infonote::

 The student wanted to change Example 3 of this lesson so that there is a new list called *eaten* where the names of the different types of food chosen by Zara will be written. To Zara, he/she added the scripts for controlling movement with arrow keys and the script shown in the figure below. The figure also shows the scripts added to other sprites in the project. Most of the events were executed as expected; however, the student was not able to write the apple and the orange into the list. Where is the bug?   

 .. image:: ../_images/9/bug9_1.png
   :width: 810px   
   :align: center

 .. reveal:: sаkrivаnjе24
   :showtitle: Show the Answer
   :hidetitle: Hide the Answer
 
   **Answer:**
     
   In the command ``wait until`` of the scripts added to the apple and the orange sprites, the sprite which should touch them is not set correctly.
      
|book| Summary
----------------

In this lesson, we learned how to use lists in Scratch - the type of data that has a complex structure, which enables multiple values to be stored at the same time. We saw that list elements could be different types of data, and that they could be used for choosing one of the costumes of a certain sprite or for choosing one of the sprites from the list of sprites. With project examples, we also illustrated the synchronization of behavior of multiplied sprites by using messages. Furthermore, we showed how the program can be used to clone sprites and how these clones can behave differently if the sprite that created them has local variables. 

**Project Examples**: 9Studio_

.. _9Studio: https://scratch.mit.edu/studios/25119484/

**New concepts**:  list, list element, clones.

**New commands**: |variables_blocks| - |add_to|,  |delete_of|, |delete_all|,  |insert_at|,  |replace_with|, |show_list|, |hide_list|, |item_of|,  |length_of|,  |list_contains|.

|control_blocks| - |when_clone|, |create_clone|, |delete_clone|. 



|project| Create a project
---------------------------

Project 1 - "History Quiz"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

Load the list of questions from a text file.

1. By using the program Notepad write a list of history questions, each question should be written in a separate row.
2. Save the text as a text file called *History.txt* with the UTF-8 encoding.

.. image:: ../_images/9/projekat9_1a.png
     :width: 250px   
     :align: center

3. In Scratch, create a list called *questions*. 
4. Right-click on the list monitor and from the shortcut menu choose the operation *import*.

.. image:: ../_images/9/projekat9_1b.png
     :width: 230px   
     :align: center

5. In the file name field write *History*
6. The list of questions you wrote previously in the Notepad will appear in your list.

.. image:: ../_images/9/projekat9_1c.png
     :width: 470px   
     :align: center

Then, create a list with correct answers and a script, which will randomly choose a question from the list of questions, ask the user to answer and then compare the answer with the correct answer from the list. If the user answered correctly, you should increase the number of his/her points.

Project 2 - "Telephone book"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

Create three lists with names, birthdays and telephone numbers of your friends. 
Write a script that checks whether the name entered from the input is included in the list. If the name is in the list, it should show the date of birth and the phone number of the person whose name was entered, and if not, the appropriate message should be displayed.

Project 3 - "Twins"
~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 3

Create procedures, which should be connected into the project Twins.

The procedure **Check** should check whether the number given as the parameter is a prime number.

The procedure **Compose** should compose a list called *Prime* where it will write every prime number from the interval [2,1000].

The main program should display all twin numbers (prime numbers that differ by 2) from the interval [2,1000].


Project 4 - Game "Dangerous Objects"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 3

Create a game where the user (a young child) should choose several objects, which are not dangerous, from the group of objects presented to him/her. The names (or sequence numbers of the costumes, like in example 4 of this lesson) of the dangerous objects on the stage should be written in the list *dangerous*.
The objects are selected by clicking on them. Then the program checks whether that parameter is included in the dangerous list. 
If the user chooses an object that is not dangerous, he/she will receive a positive point; otherwise, he/she will receive a negative point. The goal is to collect at least 3 points (out of, for example, 5). This is when the game should end, or the users should go to the next level.  

The game can have multiple levels, for example, dangers in the kitchen (knife, bowl with boiling water fire, etc.), dangers in the backyard, nature, etc. 

