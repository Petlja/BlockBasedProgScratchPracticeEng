Tell Me Where To Go - Coordinates And  Direction
================================================

.. include:: blocks.txt

.. include:: icons.txt

.. infonote::

  |intro2|

After learning the basics of the environment, it is time to learn how to send Sprites to the desired locations on the Stage. You will understand how the Stage is organized and learn the commands that allow you to move around.

.. sidebar:: Coordinates of a sprite

 |stage|

.. |stage| image:: ../_images/2/fig2_1.png

.. topic:: The Stage
      
 When Scratch starts, a Stage is automatically created: a white rectangle with 480 dots in width and 360 dots in height. The smallest dot that can be displayed on a computer graphics screen is called Pixel.

 The Stage is where your stories, games and animations will run. It is immovable, like an aquarium, but its inhabitants - the Sprites - are constantly moving and interacting. In order to easily control the movement of the Sprites, each point of the Stage is assigned an address - coordinates x and y, which represent the point's distance from the center of the Stage. The center point has the coordinates x=0 and y=0, or shorter: (0,0).

 Coordinates allow Sprites to be accurately guided around the Stage and can be brought to an arbitrary point (x, y). The Sprite's current position can be seen in the current Sprite's information.


.. topic:: Motion blocks' functions
 
 All commands regarding setting the sprites to a desired position or moving and directing are placed in the *Motion* group. The Motion group details are available in the appendix. In this chapter you are going to learn more about motion commands and **reporter blocks** through various illustrations and by doing excercises. Reporter blocks are not commands, so they cannot form a layer of a scrip alone; instead, they are used as input to other blocks. Motion reporters' function is to mantain the current coordinates and the sprite's direction.

.. topic:: Motion reporters

 In this group there are blocks |x_position| and |y_position| with the current data about the sprite's placement (about its x and y coordinates), as well as the block |direction| showing the sprite's direction. 

 To see the current coordinates of a sprite and its direction you need to click on the check block next to a desired block. If you click on the check block next to a motion reporter, a display showing current coordinates and direction will appear on the stage.

 .. image:: ../_images/2/fig2_2.png
   :width: 390px   
   :align: center
 
 
.. sidebar:: Absolute and relative commands

 An absolute command is one where the result of running the command does not depend on the current state, but only upon the values specified in the command.

 The result of running a relative command depends both upon the values specified in the command and the current state.

.. topic:: Absolute and relative motion

 You can send a Sprite to a specific spot on the Stage in two ways: by absolute and relative motion.

 **Absolute motion** is a move to a specific place - target, independent of the Sprite's current position.

 In Scratch there are 4 blocks by which a Sprite can be sent to a given position (x, y) on the Stage, or to make an absolute movement:
 
 .. hlist::
    :columns: 2

    * |goto_xy| - go to the position (x,y), 
    * |glide_xy| - glide to to the position (x,y), 
    * |set_x| - set the coordinate x of the position, 
    * |set_y| - set the coordinate y in the positions. 

 The |goto_xy| command now moves to the given position (x,y).

 Similarly, from the starting point the target will be reached with the command |glide_xy|, but the move will not happen right away, but it will take a given number of seconds. The higher the number of time for the glide, the longer it will take to get to your target. 

 Another way to set a target in absolute motion is to independently set the coordinates of x and y, using the |set_x| and |set_y| commands.

 **Relative motion** is moving to a place defined by the number of steps that the Sprite should make from the current position. Of course, you need to set direction (right, up, etc.). Another way to set a target in relative motion is to independently set the coordinates of x and y, using the |change_x| and |change_y| commands.

 You can aim the sprite to a target defined by the number of steps from its current position and to perform relative motion by the following commands:

 - |change_x| - помери се задати број пиксела хоризонтално у односу на текућу позицију, 
 - |change_y| - помери се задати број пиксела вертикално у односу на текућу позицију (х,у), 
 - |turn_right| - окрени се удесно за задати број степени у односу на текући смер, 
 - |turn_left| - окрени се улево за задати број степени у односу на текући смер, 
 - |move_steps| - помери се задати број корака у задатом смеру у односу на текућу позицију.
    

.. sidebar::  Direction blocks
   :subtitle: |point_direction| и |point_towards|

   There are two ways to set a value in the input field of the first block:

   |usmerenje1|

   (1) type in a new value, for example 45;
   (2) to rotate the blue arrow indicating the orientation in the current Sprite information.

   The |point_towards| command allows the Sprite to point to a mouse pointer or other Sprite in the project.

   |usmerenje2|

.. |usmerenje1| image:: ../_images/2/fig2_3.png

.. |usmerenje2| image:: ../_images/2/fig2_4.png

.. topic:: Direction and rotation

 In addition to the rotation commands that allow you to change orientation considering the Sprite's current direction, there is also possibility to use commands that set the orientation independently of the Sprite's current position. 

 These are  |point_direction| and |point_towards| commands. 

 You can find below the values regarding the main directions that can be set in the frst block's input field: *up* (North), *right* (East), *down* (South) and *left* (West).

 .. image:: ../_images/2/fig2_5.png
   :width: 260px   
   :align: center

 You can also set some other values, for example, 45 directs the Sprite to the Northeast, and 135 to the Southeast. To direct it to the West you do not need to use negative numbers. You can type in numbers from 180 to 360 instead.

 The second block directs the Sprite to a mouse pointer od to some other Sprite in the project. The target needs to be chosen from a drop-down list in the value field. For example, in the project "Dinosaur walk"  that will be presented later in this lesson, the cat can be directed to the mouse pointer or to one of the three dinosaurs, the Sprites of this project.
  

|study| Study the following examples
-----------------------------------------

Just like we showed an easy way for a Sprite to speak in the project "Hello World", and then we upgraded the project through the exercises so that the Sprite really pronounces the text, now we will show the basic commands for the Sprite's movement and then we’ll upgrade these possibilities through the exercises.

Example 1 - “The Walk” project
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


|1| Click on the block group *Motion*, then drag and drop |move_steps| block into the script area and click on it. The cat will move 10 steps to the right.

|2| Click on this block several times and take the cat to the right edge of the screen. 

Clicking on the move block repeatedly has allowed the action to be repeated several times. Aciton repeating can also be programmed.

|3| Return the cat to the middle of the screen and click the *Control* command group. In the Blocks palette some blocks will appear and they will be different in shape from the blocks you used - C-shaped blocks with a "mouth", in which you can insert other blocks.

|4| Select a block |forever| and drag it to the script area. Clicking on this block allows all the blocks that make part of it to run forever (until you stop running the program by clicking the stop sign).

|5| Insert a moving block into the "mouth" of the repeating block and click on it. The cat will go off screen again.

There is a way that Sprite's movement can be kept within the edge of the screen. That is an order if you're on the edge, turn around. The corresponding block is in the *Motion* group.

|6| Stop running blocks by clicking on the stop sign, then drag the block |if_edge| into the script area and place it in the "mouth" of the repeat block, behind the move block. 

.. sidebar:: Project's script

  The cat's actions are defined by the following script.

  |script|

.. |script| image:: ../_images/2/fig2_6.png

By running a script like this, the cat will constantly move from one edge to another, but it will also go upside down. Of course, there is a way to correct this as well. One is to change the way the Sprite moves in the Sprite's information, and the other is to use a motion command.

|7| Drag the motion |rotation_style| block from the *Motion* group and place it above the repeat block. Make sure that the *left-right* rotation mode is selected from the drop-down list of this block.

|8| Put the |clicked_flag| block at the beginning of the script, and you have completed “The Walk” project.

You can now start the project by clicking on |g_flag| and stop it by clicking on the |stop|. Save the project and then continue the research.

.....

У следећем пројекту показаћемо како се уводе нови ликови и позадине и како се лик води коришћењем показивача миша. Зато, пре но што пређеш на овај пример, проучи приручнике *Додај лик* и *Додај позадину*.

Example 2 – „Обилазак диносауруса”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

У претходном пројекту користили смо блок ``понављај заувек`` да постигнемо да се мачак заувек креће између рубова екрана, односно све док се не прекине извршавање пројекта кликом на на знак *стоп*. У овом пројекту учествују 4 лика и сваком од њих ћемо придружити скрипту која описује његово поношање. Мачак ће заувек да прати показивач миша, а остала 3 лика - диносауруси, ће заувек да се усмеравају ка мачку. На следећој слици приказан је изглед позорнице на почетку извршавања пројекта.

.. image:: ../_images/2/fig2_7.png
   :width: 490px   
   :align: center

**Израда пројекта**

.. sidebar:: Избор позадине

  Нову позадину можеш да додаш у пројекат кликом на дугме које се налази десно од дугмета за избор нових ликова.

  |nova_pozadina|

.. |nova_pozadina| image:: ../_images/2/fig2_8.png


|1| Кликни на дугме за избор позадина и изабери позадину *Jurassic* из библиотеке позадина.

|2| Изабери ликове *Dinosaur1*, *Dinosaur2* и *Dinosaur3* из библиотеке ликова.

|3| Ликове распореди као на слици горе. Лику *Dinosaur2* треба променити усмерење. Подразумева се да је усмерење ликова постављено на 90 :sup:`о` (гледају на десно) и да им је начин окретања *на све стране*. Ове поставке могу се променити у информацијама о лику или коришћењем одговарајућих блокова у скриптама које су му придружене. У овом пројекту користићемо први начин. 

|4| У информацијама о лику постави да начин окретања буде за лик: *Dinosaur1* - *без окретања*, *Dinosaur2* - *лево/десно*, *Dinosaur3* - *на све стране*. 

|5| Свим диносаурусима придружи исту скрипту која налаже да се све време извршавања пројекта усмеравају ка мачку. Међутим, они ће се различито понашати зато што у информацијама о лику имају постављене различите начине окретања.
   
|6| Лику мачка придружи наредбе које му омогућавају да прати координате показивача миша, односно да се по позорници креће онако како корисник помера миша. 

Скрипте које описују понашање диносауруса и мачка приказне су на следећој слици.

.. image:: ../_images/2/fig2_9.png
   :width: 600px   
   :align: center
 
Покрени пројекат и померај мачка по позорници. Обрати пажњу да диносауруси на различит начин прате његово кретање.

.....

Example 3 – "Linear motion"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|tutorial| Study the Use the arrow keys tutorial, and create a project where the cat is led around the Stage with the keyboard. 

.. sidebar:: Key selection

  The keyboard key that will run the script is selected by clicking on the white triangle next to the button name (space) and then selecting the desired race from the drop-down list. 

  |fig2_11|

.. |fig2_11| image:: ../_images/2/fig2_10.png

|1|	The Sprite cat joins |clicked_key| command.

|2| You select the *right arrow* button.
 
|3|	From the *Motion* group, select |point_direction| command and associate it with the previous command.   

|4|	From the *Motion* group, select |move_steps| command and associate it with the previous command.   

|5|	Press the right arrow key on the keyboard several times. What happens?

|6|	Duplicate this script (right click on the first command, then select *Duplicate*).

|7|	In the new script, replace the right arrow with the left arrow, and in the block ``point in direction`` instead of 90 select -90.

|8|	Press the left arrow key on the keyboard several times. What happens?

|9|	Similarly, make two more scripts: to guide the cat 10 steps up by pressing the up arrow key, or 10 steps down by pressing the down arrow key.
 
.. image:: ../_images/2/fig2_11.png
   :width: 570px   
   :align: center

.....

Example 4 – "Motion and Turn"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

We're going to do another project to run a Sprite using keyboard keys, but with modified keys settings. We will throw out directional commands, and with the left and right arrows, we will join the commands that rotate the Sprite 15 degrees left or right. With the up and down arrows we will join the commands go 10 steps, or go -10 steps. The corresponding scripts will have the following layout.
 
.. image:: ../_images/2/fig2_12.png
   :width: 555px   
   :align: center

Run the project and test how it handles movement of the Sprite's.

|ask| Did you understand?
----------------------------------

Question 1
~~~~~~~~~~

.. level:: 1

.. mchoice:: stage1
   :answer_a: 1280 steps wide and 600 steps tall
   :answer_b: 800 steps wide and 600 steps tall
   :answer_c: 480 steps wide and 360 steps tall
   :answer_d: 360 steps wide and 480 steps tall
   :correct: c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: True
   :feedback_d: 
   
   Колике су димензије позорнице?
   
Question 2
~~~~~~~~~~

.. level:: 1

.. mchoice:: stage2
   :answer_a: in the upper left corner of the Stage
   :answer_b: in the downer left corner of the Stage
   :answer_c: in the center of the Stage
   :answer_d: зависи од придружене позадине
   :correct: c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: True
   :feedback_d: 
   
   Где се налази тачка с координатама (0,0)?
   
   
Question 3
~~~~~~~~~~

.. level:: 1

.. mchoice:: blocks1
   :answer_a: Sensing
   :answer_b: Motion
   :answer_c: Control
   :answer_d: Looks
   :correct: b
   :feedback_a: 
   :feedback_b: True
   :feedback_c: 
   :feedback_d: 
   
   Којој групи  припадају блокови који управљају положајем, оријентацијом, окретањем и кретањем ликова?
   

Question 4
~~~~~~~~~~

.. level:: 1

.. mchoice:: stage3
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a:  
   :feedback_b: 
   
    Да ли позорница може да извршава наредбе кретања?

Question 5
~~~~~~~~~~

.. level:: 2

.. mchoice:: Absolute_Motion
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: a, d
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which of the commands allows absolute mmovement? (Select all correct answers)

   .. image:: ../_images/2/q2_5.png
      :width: 545px   
      :align: center

Question 6
~~~~~~~~~~

.. level:: 2

.. mchoice:: Relative_Motion
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: b, d
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which of the commands allows relative movement? (Select all correct answers)

   .. image:: ../_images/2/q2_6.png
      :width: 630px   
      :align: center

Question 7
~~~~~~~~~~

.. level:: 2

.. mchoice:: reporters
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: b, c, d
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which of the blocks represent  motion reporters? (Select all correct answers)

   .. image:: ../_images/2/q2_7.png
      :width: 335px   
      :align: center


Question 8
~~~~~~~~~~

.. level:: 3

 image:: ../_images/2/q2_4.png
   :width: 400px   
   :align: center

.. mchoice:: compass
   :answer_a: Southeast
   :answer_b: Southwest
   :answer_c: Northeast
   :answer_d: Northwest
   :correct: d
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 
   
   Which side of the world will the Sprite look at after command |2_8|?

.. |2_8| image:: ../_images/2/naredba2_8.png   

Question 9
~~~~~~~~~~

.. level:: 1

The following figure shows the positions of the 5 points on Stage.

.. image:: ../_images/2/q2_9.png
   :width: 300px   
   :align: center
      
.. mchoice:: coordinates1
   :answer_a: (-200,-40)
   :answer_b: (-200,40)
   :answer_c: (200,-40)
   :answer_d: (200,40)
   :correct: b
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 
   
   What are the coordinates of a point A?
  
.. mchoice:: coordinates2
   :multiple_answers:
   :answer_a: A
   :answer_b: B
   :answer_c: D
   :answer_d: E
   :correct: b, d
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   What points have a negative y coordinate? (Select all correct answers)


.. dragndrop:: coordinates3
    :feedback: 
    :match_1: A|||(-200,40)
    :match_2: B|||(-160,-60)
    :match_3: C|||(20,0)
    :match_4: D|||(100,120)
    :match_5: E|||(180,-80)
    
    Pair the points with their coordinates.

Question 10
~~~~~~~~~~~

.. level:: 2

The following figure shows the positions of the 6 points on Stage.

.. image:: ../_images/2/q2_10.png
   :width: 300px   
   :align: center
      

.. dragndrop:: coordinates4
    :feedback: Покушај поново
    :match_1: A|||(-160,80)
    :match_2: B|||(-160,-80)
    :match_3: C|||(160,-80)
    :match_4: D|||(80,0)
    :match_5: E|||(160,80)
    :match_6: F|||(0,80)
    
    Pair the points with their coordinates.


.. mchoice:: coordinates5
   :answer_a: Тачка А
   :answer_b: Тачка В
   :answer_c: Тачка С
   :answer_d: Тачка D
   :correct: c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   
   Which point is symmetric to point E with respect to the x-axis?

.. mchoice:: coordinates6
   :answer_a: Тачка А
   :answer_b: Тачка В
   :answer_c: Тачка С
   :answer_d: Тачка D
   :correct: a
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 
   
   Which point is symmetric to point E with respect to the y-axis? 


.. mchoice:: coordinates7
   :multiple_answers:
   :answer_a: A и B
   :answer_b: A и C
   :answer_c: A и E
   :answer_d: D и F
   :correct: a, b, c
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which points are equidistant from the y-axis? (Select all correct answers) 

|try| Try it!
-----------------

Exercise 1 - Tracking the position of the Sprites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

.. infonote::

  |1| Drag the cat Sprite to the upper left corner of the Stage, and then check the Sprite information for the coordinates of the point at which you left it.

  |2| Then drag it to the upper right corner of the Stage and check again the coordinates of the point where you left it.

  |3| Repeat the previous procedure for the points in the lower corners of the Stage. At what points on the Stage did the coordinate x have a minus sign and at which coordinate y was negative?

  |4| Import an Apple Sprite from the Sprite library. A blue frame should appear around the thumbnail of a new Sprite in the Sprite list, which means that the Sprite is in focus. If not, click on its thumbnail in the Sprite list.
       
  |5| Check the variables *x position* and *y position* at the bottom of the block group *Motion*. *Apple: x position* and *Apple: y position* will appear on Stage.

  |6| It now drags the Apple Sprite to different places on the Stage and monitors how its coordinates change.

.....

Exercise 2 - Setting the position of a Sprite with absolute motion commands
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|tutorial| Before doing this exercise, study the *Add a Backdrop* tutorial.

.. level:: 2

.. infonote::

  |1| Click on the Stage picture next to the list of Sprites. A blue box will appear around the Stage image, so the Stage is in focus.

  |2| Click the |b_back| button, and from the Backdrop library window that opens, select the  *Xy-grid*.

  |3| Now click on the |code| Code tab to get a block palette instead of a |costume| Backdrops tab.

  |4| You will get the message *Stage selected: no motion blocks* in the *Motion* group, which is understandable because the Stage that is now in focus can't move.
  
  |5| Click on the cat Sprite in the Sprite list. When a blue frame appears around the thumbnail, blocks of the *Motion* group will return.

  |6| Drag the |goto_xy| block into the script area, then change the value of x to 120 and the value of y to 100.

  |7| Click on the modified block in the script area. What happened?

  |8| Drag the |glide_xy| block into the scripting area, then change the value of x to -120 and the value of y to 100. What happens when you click on this block?

  |9| Follow where to find the Sprite after clicking on a block where you previously typed different values for x and y. For example, where will the Sprite be if both coordinates are negative, if off Stage etc.

.....

Exercise 3 - Absolute and relative motion
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 3

.. infonote::

  Try to guide the Sprite from point A to point B by using different *Motion* commands.
   
  |1| Set *Хy-grid* from the Backdrop library as the bacdrop.

  |2| Select two new Sprites from the Sprite library - letters A and B (Block-A and Block-B).
  
  |3| Set the letter A in the lower left corner of the Stage to the position (-200, -120), and the letter B in the upper right corner to the position (200,120). This is most precisely done by assigning the letter A to the go_xy block (dragging it into the script area while the letter A is in focus), entering the appropriate coordinates x and y, and clicking on the block. Repeat the procedure for the letter B.
  
  |4| Join the cat with the |goto| command and select Block-A from the drop-down list (which you will get when you click on the white triangle in the selection box). **Note**. |goto| |!=| |goto_xy|. 
   
  |5| Click on the |goto| block and the cat will be located below the letter A.
  
  |6|  Click on the |goto_layer| from the *Looks* group and Cat will be located above the letter A.
  
  .. image:: ../_images/2/ex2_3.png
     :width: 220px   
     :align: center

  |7| Now in block  |goto| choose *Block-B*, then click on it. The cat will immediately find itself above the letter B.

  |8| The cat is joined by a block |glide_to|, and select *Block-A* from the drop-down list, then click on it. The cat will move up to the letter A for 1 second. **Note**.  |glide_to| |!=| |glide_xy|. 

  |9| Now select *Block-B* from the drop-down list and set a longer glide time, for example 5 seconds. Click on the block.
    
  |10| Try the third way. First, the cat joins the block |point_towards|, and from the drop-down list chooses to point to the Block-A Sprite. **Note**.  |point_towards| |!=| |point_direction|

  Click on the |move_steps| block until the cat reaches letter A.

.....

Exercise 4 - Commands for rotation style and direction
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Направи пројекат у коме ће се ликови понашати потпуно исто као у пројекту „Обилазак диносауруса”, али немој вршити измене у информацијама о лику. Уместо тога, начин окретања и усмерења ликова постави у скриптама придруженим ликовима. Упамти овај пројекат под називом „Обилазак диносауруса2”

.....

Exercise 5 - Adding new Sprites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Iскористи пројекат „Шетња” за креирање новог пројекта у који ћеш увести нови лик. То може да буде, на пример, пас или миш, који све време треба да се усмерава према мачку. Додај позадину по избору. У скрипти која описује понашање новог лика задај и начин окретања. Немој вршити измене у скрипти придруженој мачку. Упамти овај пројекат под називом „Шетња2”.

|bug| Debug it!
--------------------

Bug 1
~~~~~~~~

The pupil wanted to make a simple animation of the cat's movement by changing his costume. So he joined him with the following script. 

.. image:: ../_images/2/bug2_1.png
    :width: 220px 
    :align: center

However, nothing was happening. What was the mistake?

Bug 2
~~~~~~~~

The pupil wanted his Sprite to step between the left and right edges of the Stage. That is why he put in an endless cycle of constantly changing costumes and stepping 10 steps until he reaches the edge of the Stage as he turns. However, he didn't like the Sprite stepping upstairs to the left edge of the Stage. What should he do to fix this error?
  
  
|book| Summary
----------------

У овој лекцији смо показали како се помоћу две координате може прецизно одредити положај тачке на позорници. Ликове можемо послати на задату локацију наредбама апсолутног и релативног кретања. Апсолутно кретање је померање на одређено место – одредиште, независно од тренутне позиције лика, док је релативно кретање померање на место које је од тренутне позиције лика удаљено задати број корака у задатом смеру. Позорница не може да извршава наредбе кретања. Кроз примере пројеката и вежбе показали смо како се кретањем ликова може управљати диркама  тастатуре и помоћу миша.

**New concepts**:  pixel, coordinate system, coordinates, motion commands, motion reporters, absolute motion, relative motion, orientation, rotation mode.

**Strach commands**: |motion_blocks| - |move_steps|, |turn_right|, |turn_left|, |point_direction|, |point_towards|, |goto_xy|, |goto|,  |glide_xy|, |glide_to|, |set_x|, |set_y|, |change_x|, |change_y|, |if_edge|, |rotation_style|, |x_position|, |y_position|, |direction|; |events_blocks| - |clicked_key|; |looks_blocks| - |*| |goto_layer|,  |*| |switch_costume|; |control_blocks| - |*| |forever|.

Note. commands marked with the |*| sign will be discussed in the  lessons that follow.

|project| Create a projects
----------------------------

Project 1 - “Two Players”
~~~~~~~~~~~~~~~~~~~~~~~~~

Start a new project that you will call “Two Players”. Put two Sprites on the Stage, one on the left and the other on the right. Set the Sprites to be pointing at each other. Join Sprites with scripts that allow them to *Motion* back and rotate clockwise and counterclockwise.

The control keys for the first Sprite should be:

- Up Arrow - The Sprite goes straight ahead,

- Down Arrow - The Sprite goes straight back,

- Left arrow - The Sprite rotates counterclockwise,

- Right arrow - The Sprite rotates clockwise.

The control keys for the second Sprite should be:

- Button W - The Sprite goes straight ahead,

- Button S - The Sprite goes straight back,

- Button A - The Sprite rotates counterclockwise,

- Button D - The Sprite rotates clockwise.

