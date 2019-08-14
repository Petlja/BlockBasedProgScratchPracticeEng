My First Program
================

.. include:: blocks.txt

.. include:: icons.txt

.. infonote::

  |intro1|

   
Would you like to create your own computer game, animated story, instruction or a presentation? Scratch is a programming language that enables you to create all of the above, and even more.

Unlike the most common programming languages, Scratch is a *visual* programming language – instead of typing the commands, you can program in Scratch by snapping color-coded blocks together like LEGO bricks.

In Scratch, **projects** are created. The first step in creating a project is adding the sprites that will participate in it. Different outlooks, sounds and behaviors can be linked to all of the sprites. The behavior of a sprite is described by the **script**. The project contains one or more scripts, each of which is associated with a sprite or a stage - the place where the project takes place.

In order to write a program in Scratch, it is necessary to get to know the environment in which the programs are created, or its **interface**.

.. topic:: Scratch Programming Environment

 The following Figure shows the interface of the Scratch programming language. 

 .. image:: ../_images/1/fig1_1.png
   :width: 800px   
   :align: center

 First, we will learn about the basic functions of its main parts, and in the following lessons we will get to know other components of the environment.

 **The Stage** is a place where your sprites move, draw and interact. The stage itself is immovable, but it has sprites on it that can be moved and interacted with other sprites.

 **The Block Palette** is an area where all of the available orders of the Scratch programming language are placed. It is called “the palette” because it looks like a palette which the painter uses to paint. Unlike the painter, the programmer creates live pictures with objects that interact with each other.

 **Scripts Area** is a place where the scripts are created. To make a script, you need to drag blocks from the block palette to the Scripts area and snap them together.

 **The Sprite List** displays names and thumbnails for all the sprites in your project.

 **The File Menu** allows you to set project management commands and adjust the environment itself.

.. topic:: My First Program

 Even the longest journeys begin with one first step. And that first step in learning a programming language is to write a program that displays "Hello World" on the screen. And that is how we will start conquering Scratch.

 Whenever Scratch is launched, a new project is created and it contains white Stage and a Cat Sprite.

 Stage and Sprites are **objects** whose behavior is programmed by Scratch commands. We build scripts describing the objects behavior by using blocks which correspond to language commands. Each object has its own behavior, even a fixed stage that, for example, can change its backdrop.

 Stages and Sprites can be associated with **graphics** (pictures - drawings, photos) and **sound** files in addition to scripts. Sprite pictures are called costumes, and stage pictures - backdrops.

 **The Sprite list** shows thumbnails of all the Sprites involved in the project. Each Sprite's name is writen in the bottom.

 You can view and modify the current Sprite information in the space above the Sprite list.

 .. image:: ../_images/1/fig1_2.png
   :width: 650px   
   :align: center
 
 .. infonote::

  1. The name of the Sprite can be changed by typing a new name in the Sprite's name field.

  2. The position of the Sprite on the stage is given by its coordinates x and y.

  3. Whether the Sprite is visible or hidden from the Stage depends on what is checked in the Show checkbox.

  4. The size of the Sprite is expressed as a percentage of the original size. The number 100 indicates that the Sprite is at its normal size.

  5. The direction indicates the direction in which the Sprite will move. The blue arrow on the circle shows the direction of the Sprite. You can change the orientation by rotating the arrow or typing the appropriate number in the direction field (0: up, 90: right, 180: down, -90: left). The rotation style indicates the rotation mode, which can be: *All Around*, *Left/Right*, or *Do not rotate*.

 To create a script, you need to drag the appropriate commands from the command palette to the script area for the active object, and to link them.

 **An active object** - a Sprite or a Stage, is recognized by the fact that there is a blue box around its thumbnail in the Sprite list. Everything we create: scripts that describe behavior, costumes that describe the look, sounds that will be heard when we start a project, is beeing conected to the object that is active.

 Creating scripts is done by placing blocks one the top of the other. Clicking anywhere within a series of blocks launches a complete script that runs from the top to the bottom.  

|study| Study the following examples
-------------------------------------

Example 1 - The “Hello World” Project
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The simplest possible script, which consists of a single command - a block that allows the Sprite to say text "Hello world" will be attached to the cat. After that, when you click on the block, the text will appear in a speech bubble. 

Let's do it!

|1| Click on the block group *Looks* in the block palette. A group of purple blocks for visual effects will appear. 

|2| Drag the |say_sec| block to the script area. 

|3| Then instead of text *Hello*, type *Hello World* and click on the modified block.

.. image:: ../_images/1/fig1_3.png
   :width: 480px   
   :align: center

“Hello World” text will stay on the Stage next to the cat for 2 seconds. As you can see, quite simple.

Now we are going to add a few more  ``say`` blocks to make our Sprite say a few more sentences. 

We will show two ways to add a block that already exists in the script area. 

- 1. By repeating the procedure we have already done: drag an another ``say`` block  from the block palette and instead of the text „Hello“ type „I'm a cat“.

- 2. Right-click on the block in the script area to open the shortcut menu and select  *Duplicate* from it. Then, in the copy of the block, enter the text you want, in our example – „I like to walk“. In this way you can work faster, as you can multiply stacked blocks that have been previously connected one to another.

.. image:: ../_images/1/fig1_4.png
   :width: 500px   
   :align: center
 
To make the blocks run automatically one after the other, you need to put them together in a stack. We do this by dragging blocks. When the blocks are close, a shadow appears bellow the block, indicating that the blocks will be connected. By connecting all three blocks in the stack,  after double clicking on it, the Sprite will say all three sentences, one after the other. 

**Running project**

You noticed that the block you used has a notch at the top and a bump on the bottom. A block of this shape is called a **stack block**. Most of the commands are performend by stack blocks. However, the first block that indicates which event will trigger the script, are shaped with a rounded top, as there are no blocks that precede it. These blocks are called **hat blocks** and most of them can be found in  the *Events* group. Click the *Events* group in the block palette and drag the |clicked_flag| block to the script area. Then place this block on top of the previously formed stack and your first project is done. To run it click on |g_flag| above the top left corner of the stage. 

**Saving project**

You can save the project to your computer as follows.

|1| Click *File* in the menu bar.

|2| Select *Save to your computer* from the options.

|3| In the dialog that opens, select the folder and enter the name of your project, then click on the *Save* button.

**Upgrading project**

Instead of displaying a speech bubble with a text, a cat could actually pronounce this text. You can do this by selecting the 
|play_until| block from the *Sound* group, and in the sound editor, record the sentence you want to say. Then in the block ``play sound`` instead of sound "meow", select the recorded speech. 

In this version of Scratch you can do more than that. Among the extensions, there is a *Text to Speech* group that allows Sprites in projects to start speaking for real. You can do it only if you are connected to the Internet because it uses *Amazon Web Services*. 


|ask| Did you understand?
----------------------------

Let's try to answer some questions that have not been explained yet! Simply start Scratch and go!

Question 1
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface1
   :answer_a: script
   :answer_b: object
   :answer_c: interface
   :answer_d: program
   :correct: c
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 
   
   The name for all windows and buttons that are visible when you launch Scratch is?
  

Question 2
~~~~~~~~~~
.. level:: 1

Some parts of the Scratch interface in the following figure are numbered from 1 to 5. 

.. image:: ../_images/1/q1_2.png
   :width: 600px   
   :align: center
      
.. dragndrop:: interface2
    :feedback: Покушај поново
    :match_1: позорница|||4
    :match_2: палета наредби|||2
    :match_3: област скрипти|||3
    :match_4: листа ликова|||5
    :match_5: линија менија|||1
    
    Drag the name of each environment part to the number corresponding its position in the image.


Question 3
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface3
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a:  Project needs to have а stage with at least one backdrop.
   :feedback_b: 
   
   Is there a project without a stage?

Question 4
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface4
   :answer_a: yes
   :answer_b: no
   :correct: a
   :feedback_a:  
   :feedback_b: It is possible that a project has only scripts for the stage.
   
   Is there a project without sprites?


Question 6
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface6
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a:  Some sprites can be only decoration of the project.
   :feedback_b: 
   
   Does every project sprite need to be associated with at least one script?


Question 8
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface8
   :answer_a: линија менија
   :answer_b: листа ликова
   :answer_c: област скрипти
   :answer_d: палета наредби
   :correct: b
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 
   
   How do we call the place where we can find the sprites thumbnails?  

Question 9
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface9
   :answer_a: look
   :answer_b: suit
   :answer_c: costume
   :answer_d: mask
   :correct: c
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 
   
   You can change the appearance of a sprite by choosing a different: 

Question 10
~~~~~~~~~~~

.. level:: 1

.. mchoice:: interface10
   :multiple_answers:
   :answer_a: presentations
   :answer_b: scripts
   :answer_c: graphics files
   :answer_d: sound files
   :correct: b,c,d
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   What can be assigned to the stage and to sprites? (Select All the Correct Answers)  



It's time to explore.

|try| Try it!
-----------------

Exercise 1 - Exploring the Tutorials
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

By clicking the Tutorials button |tutorial| from the menu bar (1) you will open a library of short instructions for creating different projects in Scratch. Then select the Tutorial First Steps (2), watch the associated video (3). By clicking on the green arrow (4), you can review the steps for making simple projects similar to our project "Hello World".

.. image:: ../_images/1/ex1_1.png
   :width: 1000px   
   :align: center

.....

Exercise 2 - Sprite Information
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

|1| In the current Sprite information, change the direction of movement of the Sprite so that it goes up. What will happen on stage?

|2| How will the Sprite be directed if you set a value of 45 degrees as the direction of motion?

|3| Hover your mouse over the Sprite and track what's happening with the coordinates in the current Sprite information.

|4| Check what's going on with the Sprite if the Show box indicates that the Sprite is hidden? How can you get a Sprite back on stage?

|5| Change the name of the active Sprite.

.....

Exercise 3 - Introducing New Sprites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
      
.. level:: 1

.. sidebar:: Choose a Sprite
    
    You can add a new Sprite to the project by clicking the button |b_sprite| at the bottom right of the Sprite list.

    |new_sprite|

.. |new_sprite| image:: ../_images/1/fig1_5.png
  
|1| Import a new Sprite from the Sprite library. By clicking the Select button you will open the Sprite library window. You need to click on the Sprite you want to choose - for example, the ballerina Sprite. 

|2| Draw a new Sprite using the built-in image editor. By clicking the Draw button instead of the Program tab opens the Costumes tab. At the place where the script area was, a graphic editor where you need to draw a new Sprite will be opened. When you're done, click the Program tab.
  
|3| Import a few surprise Sprites from the Sprite library.

|4| Import a new Sprite from a file by clicking Upload Sprite.

.....

Exercise 4 - Duplicating and Deleting Sprites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

|1| Right-click on a Sprite in the Sprite list to open the shortcut menu. Multiple the Sprite by making 3 copies.

|2| Remove one of the Sprites' copies by selecting Delete from the shortcut menu.

|3| By entering numbers 50 and 200 in the size box, set one copy to be twice as small and the other as twice as large as the original.

.....

Exercise 5 - Using Sound  
~~~~~~~~~~~~~~~~~~~~~~~~~

.. warning:: You can only do this exercise if your computer has audio recording capability! 

Explore the Tutorial Record sound, and try to create a project where the Sprite will say the phrase "Hello World" by your voice. As this exercise uses a sound editor which we will introduce later, you can skip it at this point.

.. level:: 2
 
|1| Start Scratch.

|2| Click on the Sound commands in the block palette. A group of light purple blocks for the sound effects that can be assigned to the Sprites will appear.
  
|3| Drag |play_until| block to the script area. 
  
|4| Click on the Sounds tab. The Sound Editor window will open.
  
|5| Click on the Choose a Sound button and select the recording option.

|6| When the Recording dialog box appears, click on the record button, then say the phrase "Hello World" and stop recording.

|7| Listen to the recording and if you like it, click Save. Another sound named *recording1* will appear in the list of sounds associated with the cat Sprite.

|8| Return to the Programs tab and select *recording1* instead of the *meow* sound. If you click on the green flag, the cat will say the sentence you recorded.

|9| Add two more blocks  |play_until|, then add to them a snapshot of the other two sentences spoken by the cat.

|10| Connect the blocks to the stack and place |clicked_flag| block at the top. 

|11| Save this project as "Hello World2".

.....

Exercise 6 - Using Text-to-Speech Extensions  
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. warning::  You can only do this exercise if your computer is connected to the Internet! 

Explore the Tutorial  Create Animations That Talk, so try to create a project where the Sprite will say the phrase "Hello World" using a block of speech. This exercise also uses the commands we will discuss later. 
 
.. level:: 3
 
|1| Start Scratch.

|2| Click on the button |extensions| at the bottom of the block palette. Extension block groups will appear.
  
|3| From the Add Extensions group, you need to select |voices_extension|. Three new blocks will appear in the block palette. Thanks to these blocks the Sprite will reproduce the text written in command input field |speak|, in the language set by  |set_language| command. You can also set the voice to: female (soprano or alt) or male (tenor or bass). This is set by |set_voice| command.  
  
|4| Drag the block |set_language| to the script area. 
  
|5| Drag the block |set_voice| to the script area and choose how the voice of the Sprite would sound like.
  
|6| Drag the block |speak| to the script area and type in "Hello World" in its input field . 

|7| Add two more blocks to speak, then type in the other two sentences spoken by the cat.

|8| Connect the blocks to the stack and place |clicked_flag| block at the top.

|9| Save this project as "Hello World3".

|bug| Debug it!
---------------

Bug 1
~~~~~

The pupil wanted to make his own version of the project "Hello World". In it, the Sprite should say one sentence after another: "Hello World", "My name is Mike", "I like programming". He attached the Sprite to the following script.

.. image:: ../_images/1/bug1_1.png
     :width: 220px   
     :align: center

But after clicking on the green flag, the Sprite said only "I like to program". What's the mistake?

|book| Summary
-----------------

This lesson provided a high-level overview of Scratch and its programming environment. We have written, run and saved our first project "Hello world". We did exercises on how to make sprites reproduce sentences that we register through the sound editor and those uoploaded from the Text-to-Speech extention (only if the comuter is connecte to the Inernet).

**New concepts**:  Interface, Project, Sprite, Costume, Stage, Backdrop, Script, Instruction.

**Strach commands**: |events_blocks| - |clicked_flag|; |looks_blocks| - |say_sec|,  |say|; |sound_blocks| - |*| |play_until|; |voices_extension| -  |*| |set_language|,  |*| |set_voice|,  |*| |speak|.


Note. Instructions marked with the |*| sign will be discussed in the  lessons that follow.

|project| Create a project
---------------------------

Project 1 - „About Me”
~~~~~~~~~~~~~~~~~~~~~~~~

Create a project which will represent you. Choose a boy or a girl Sprite from the Sprite library and attach a script that will make the sprite say the following three sentences: "My name is ...", "I'm ... years old" and "My school name is ...". Insert your data instead of dots.

