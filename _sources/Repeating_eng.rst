Repeating steps
===============

.. include:: blokovi.txt

We saw that the stage is 480 points wide and 360 points high, and that each of the stage's points can be accessed using its coordinates. In the following examples, we will create images by leaving a character stamp in the given positions. Of course, we can create any character we like in the graphic editor - for example, a red circle or a blue square, but in order to make the images more attractive, in our examples, we will use the *Star* character - a yellow star from the character library.

To better fit the character images on the stage, we will slightly change the star size. The original size is :math:`47 \times 48` pixels, which can be seen if we go to the *Costumes* tab (fig. 5_1). It's more convenient for us that the star size is :math:`40 \times 40` pixels, because then we can place exactly 12 stars (:math:`{480 \over 40} = 12`) in one row (from left to right), and we can place exactly 9 stars (:math:`{360 \over 40} = 9`) in one column. Furthermore, it is more suitable for us if our character had no contour and if it were completely uniformly filled with one color.

.. image:: ../_images/5/sl5_1.png
   :width: 700px   
   :align: center


.. infonote::

  How to Change the Character *Star*

    1. Select the entire character with the selection tool

    2. Remove the contour (set its thickness to 0)

    3. Select an inner star and delete it

    4. Select the whole character and set it's size to 40x40.

.. image:: ../_images/5/sl5_2.png
   :width: 700px   
   :align: center

This modified star will be the only character in the following tasks.

|prouci| Tasks
---------------

.. |prouci| image:: ../_images/prouci.png

.. questionnote::

   1. Write a program that will draw 4 stars of different colors, each 120 pixels big, one next to the other, and they should fit the window, edge to edge, as in the following picture. 
   
.. image:: ../_images/5/slika1.png
   :width: 495px   
   :align: center

We can solve the task with the following steps:

1. Increase the size of the character to 300%, so now, the star is :math:`120 \times 120` pixels,
2. Set the character so that it's left edge is on the left edge of the stage: :math:`x = -180`
3. Put a stamp
4. Move the star to the right for its width (120 steps)
5. Change the color of the character (the "Change color effect" command)
6. Put a stamp
7. Move the star to the right for its width (120 steps)
8. Change the color of the character (the "Change color effect" command)
9. Put a stamp
10. Move the star to the right for its width (120 steps)
11. Change the color of the character (the "Change color effect" command)
12. Put a stamp

We see that we repeated the steps 4-6 3 times. The program that corresponds to this description is shown in the following figure.

.. image:: ../_images/5/zvezda1.png
   :width: 235px   
   :align: center

.. questionnote::

   2. Write a program that will draw 12 stars of 40x40 size, one next to the other, from the left to the right egde of the screen, as in the following figure.

.. image:: ../_images/5/slika2.png
   :width: 490px   
   :align: center

This task is similar to the previous one, just without a need to enlarge the size of the character. We should first send it to :math:`x = -220, y = 0`, and put a stamp. Then, we should repeat 11 times the steps 4-6 of the previous program, with the character moving 40 instead of 120 steps. But how much time would it take to make this simple program?

It would certainly be faster, after making the first stamp, to repeat steps 4-6 again 11 times automatically somehow. In Scratch we can do this using the "repeat" block.

The *repeat* block allows us to write a group of repeated commands only once and set how many times they need to be repeated which looks like this: | repeat10 |

This is an example of the so-called C-blocks, blocks that resemble the letter C with their appearance. The slot within the C-block is a special type that receives a script as an input. This block has 2 inputs: one for the number of reps and one for the script.

The solution to the task is shown in the following figure.

.. image:: ../_images/5/zvezda2.png
   :width: 265px   
   :align: center

.. questionnote::

   3. Write a program that draws 15 stars of different colors one over the other in the center of the screen, where the first should be :math:`320 \times 320` (800% of the original size), and every next star is smaller for 50% of it's original size, than the previous picture, as in the following figure.


.. image:: ../_images/5/slika3.png
   :width: 700px   
   :align: center

When we say 50% smaller we mean 750%, 700%, ... of the original size (not 50 pixels smaller, nor 50% of 800%). In order to avoid mixing the image with possible image residuals from previous execution of the program, we will initially place the "erase all" command.

The solution to the task is shown in the following figure.

.. image:: ../_images/5/zvezda3.png
   :width: 265px   
   :align: center

.. questionnote::

   4. Write a program that will draw a frame around a stage, composed of the stars of different colors as in the following figure.

.. image:: ../_images/5/slika4.png
   :width: 490px   
   :align: center

Solving this task can be achieved by linking the solutions of the 4 simpler problems.

1. Draw stars on the top edge of the stage from left to right.
2. Draw stars on the right edge of the stage from top to bottom.
3. Draw stars on the bottom edge of the stage from right to left.
4. Draw stars on the left edge of the stage from bottom to top.

The first problem has already been solved in task 2. It is only necessary to change the value for the initial position of the star, instead :math:`y = 0` we should set :math:`y = 160`.
The easiest way to solve the second problem is to first change the orientation of the character, since now it should move down instead of right. The "move" block, "change color" block, and the "stamp" block should be repeated 8 times.
The third and fourth problems are solved in a similar way, only the orientation of the character is changed, and we should calculate how many times it should make a stamp. Part of the solution is shown in the following figure.

.. image:: ../_images/5/zvezda4.png
   :width: 780px
   :align: center

The structure of the solution to this task, in which one loop follows another, is called the **linear compsition of loops**.

.. questionnote::

   5. Write a program that will draw 4 stars, each 120 pixels big, one next to the other, arranged from the left to the right edge of the screen. Each of these 4 stars should consist of several stars of different sizes and colors like the star from task 3.
   
We expect the end result to be as in the following figure.

.. image:: ../_images/5/slika5.png
   :width: 490px   
   :align: center

The solution to this task also has a complex structure, but it needs to nest a loop that prints smaller stars over larger ones as in task 3, in a loop that is executed 4 times and draws large stars one next to another as in task 1. The complete solution is shown in next picture.

.. image:: ../_images/5/zvezda5.png
   :width: 300px   
   :align: center

The structure of the solution of this task, in which the loop is embedded in another loop, is called the **nested loop composition**.

|pitaj| Answer the following questions
--------------------------------------

.. |pitaj| image:: ../_images/pitaj.png

Question 1
~~~~~~~~~~

.. mchoice:: for01
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: a, b, d
   :feedback_a: The character makes :math:`10 \times 8 = 80` steps.
   :feedback_b: The character makes :math:`10 \times (5 + 3) = 80` steps.
   :feedback_c: The character makes :math:` 2 \times 10 + 5 \times 10 = 70` steps.
   :feedback_d: The character makes :math:` 5 \times 10 + 10 + 2 \times 10 = 80` steps.
  
    Which of the counting loops move the character 80 steps? (Select All the Correct Answers).

   .. image:: ../_images/5/for01.png
      :width: 700px   
      :align: center

Question 2
~~~~~~~~~~

.. mchoice:: for02
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: b, c, d
   :feedback_a: The character makes :math:` 5 * 8 = 40` steps.
   :feedback_b: The character makes :math:` 8 * 10` steps.
   :feedback_c: The character makes :math:` 10 * (5 + 3)` steps.
   :feedback_d: The character makes :math:` 5 * 2 * 8` steps.
   
  Which of the counting loops move the character 80 steps? (Select All the Correct Answers).

   .. image:: ../_images/5/for02.png
      :width: 700px   
      :align: center


|pokusaj| Try
-----------------

.. |pokusaj| image:: ../_images/pokusaj.png

Exercise 1
~~~~~~~~~~

.. infonote::

  **Open necklace**. Create a project that displays a series of circles of different colors and sizes starting from the left end of the stage.
  
  .. image:: ../_images/5/boja1.png
      :width: 240px   
      :align: center

.. reveal:: упутство2_eng
   :showtitle: Show hint
   :hidetitle: Hide hint

   **Hint:**
 
   The image is obtained just by putting the pen down at different positions. The pen should change colors, should have the thickness 80, and it should be held by a hidden character, which is initially in the position (-200, 0). In a loop that repeats 5 times, the character should go 80 steps with a raised pen, increase the number of pen color by 30, and then put it down. The initial value for the pen color is 0. Ensure that the previous drawing is cleared by clicking on the green flag.

Exercise 2
~~~~~~~~~~

.. infonote::

  **Closed necklace**. Create a project that draws a closed set of 12 circles of different colors, each circle with the thickness of 50.
   
  .. image:: ../_images/5/boja2.png
      :width: 200px   
      :align: center 
      
  .. reveal:: упутство3
     :showtitle: Show hint
     :hidetitle: Hide hint
 
     **Hint:**
   
     The image is obtained by putting the pen down at different positions. The pen should change colors, should be have the thickness of 50, and it should be held by a hidden character, which is initially in the position (-50, 50). In the loop that repeats 12 times, the character should go 50 steps with a raised pen, turn 30 degrees and increase the value of pen color by 15, then leave a trace. The initial value for the color is 0. Ensure that the previous drawing is cleared by clicking on the green flag.

Exercise 3
~~~~~~~~~~

.. infonote::

  **A set of circles**. Create a project that displays a series of circles of different colors and sizes starting from the left end of the stage.
    
  .. image:: ../_images/5/krugovi1.png
      :width: 240px   
      :align: center
      
  .. reveal:: упутство4
     :showtitle: Show hint
     :hidetitle: Hide hint
 
     **Hint:**
  
     The image is obtained similarly to the previous exercises. The initial position of the (hidden) character is (-200, 0). The initial values are 0 for pen color and 80 for pen thickness. In the loop that repeats 5 times, the value of the pen color should be increased by 30 and its thickness should be decreased by 10. The character should go 80 steps to the right, with the pen raised, of course. The loop should also contain the *wait* command, so you can better follow what's going on. Ensure that the previous drawing is cleared by clicking on the green flag.

Exercise 4
~~~~~~~~~~

.. infonote::

  **Concentric circles**. Create a project that displays a series of concentric circles of different colors in the center of the stage.
    
  .. image:: ../_images/5/krugovi2.png
      :width: 200px   
      :align: center
      
  .. reveal:: упутство5
     :showtitle: Show hint
     :hidetitle: Hide hint
 
     **Hint:**
     
     The image is obtained by putting down the pen of different thicknesses and different colors. The pen is held by the hidden character located in the center of the screen. In the loop that repeats 8 times, the value of the pen color should be increased by 25 and its thickness should be reduced by by 30. The initial values are 0 (red) for the color and 240 (the thickest) for the thickness.
     
     The loop should also contain the *wait* command, to better follow what's going on. After each change in the value of pen's attributes, the pen should be put down. Ensure that the previous drawing is cleared by clicking on the green flag.
 
|bug| Fix the bugs
------------------

.. |bug| image:: ../_images/bug.png

Bug 1
~~~~~

:Question:
   A pupil wanted his character to walk between the left and right edgee of the stage. That's why he made an endless loop, with costume changes and walking 10 steps inside the loop, until he reached the edge when he was supposed to turn. However, he did not like that the character walks upside down on the left edge of the stage. What should he do to fix this bug?
   
.. image:: ../_images/5/greska5_1.png
   :width: 210px   
   :align: center   
   
.. reveal:: сакривање10
   :showtitle: Show answer
   :hidetitle: Hide answer
 
   **Answer:**
   
   The bug can be fixed by inserting the |nacin_okretanja| command in the character script.
   
Bug 2
~~~~~

:Question:
   A pupil wanted that his butterfly character, which had two costumes - with raised and lowered wings, to constantly glide, waving his wings between the points with the coordinates taken randomly. But his program did not do it. The butterfly slid from one to the other point either with the lowered or with the raised wings. What's wrong?
   
.. image:: ../_images/5/greska5_4.png
   :width: 285px   
   :align: center
   
     
.. reveal:: сакривање8
   :showtitle: Show answer
   :hidetitle: Hide answer
 
   **Answer:**
     
   It was necessary to make two scripts running simultaneously.

   .. image:: ../_images/5/resenje5_4.png
      :width: 460px   
      :align: center   


|knjiga| What we learned
------------------------

.. |knjiga| image:: ../_images/knjiga.png

Through previous examples and exercises, we've met the repetition orders. The simplest example of a repeat command is the command to describe the so-called. "endless loop". Repeated commands constitute the **body of the cycle**. Their execution can be stopped only by terminating the program.

.. image:: ../_images/5/ponavljaj.png
   :width: 350px   
   :align: center

For example, if we want to achieve the illusion that a cat is walking, a ballerina is dancing, or a butterfly is flying, it's enough to add each of them a script that repeats the orders |sledeci_kostim| and |cekaj| in the infinite loop.

Of course, the character should have at least two costumes and the waiting should be short, for example 2 tenths of a second (0.2). The "wait" order between displaying different character costumes is necessary in order to notice the changes in the appearance. Namely, the human eye is not able to register such a rapid changes as those that the computer performs. That's why we use "wait" commands to slow down the displaying of the next look, until our eye accepts the previous image.

In the examples of drawing, we used the so-called. "counting loops". These are repetitions where you know in advance how many times the body of the loop will be performed.

.. image:: ../_images/5/ponovi_n.png
   :width: 380px   
   :align: center

In Scratch there is a command for a loop whose number of repetitions is not known in advance, but depends on whether the condition for leaving the loop is fulfilled.

.. image:: ../_images/5/ponovi_uslov.png
   :width: 390px   
   :align: center

The requirement to skip commands of the body of the loop (the exit condition) is checked at the beginning of each loop, so it may happen that the loop body is not executed even if this condition is fulfilled at the first check. It may also happen that the cycle is executed infinitely if the condition for exiting the cycle is never fulfilled.

|project| Create a project Hungry shark
---------------------------------------

.. |project| image:: ../_images/project.png


Make a project in which the main character - shark, will fish. Download all characters (shark and 3 fish) and the background from the library of characters and backgrounds. The shark has three costumes, so its reaction when you send it to the prey by pushing the space key can be more effective than the witch reaction (which only screamed when she plunged at the ghost). Make the shark cruise from left to right endlessly, and make the fish that were eaten reappear again after 3-5 seconds. The different duration of the intermission between the two occurrences of the fish and the different place they appear will be provided by using the *random number* operation.
