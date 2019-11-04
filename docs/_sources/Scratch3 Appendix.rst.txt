Appendix
==========

.. include:: blocks.txt

.. include:: icons.txt

.. infonote::

  |intro11s|

Block Functions
----------------

In Scratch, the shape of a block ensures that, when the blocks are connected, they can form only scripts, which are syntactically correct. There are independent blocks and function blocks. Independent blocks (hat blocks, stack blocks, C-blocks, and cap blocks) correspond to language commands. Function blocks (reporters and logical blocks) store values of independent blocks. In lesson 3, we talked about the different types of blocks, and now we will introduce the functions of main block groups and some of the groups located in the part Extensions. 

Motion Blocks
~~~~~~~~~~~~~~~~

.. sidebar:: |motion_blocks| Motion
    
   |fig11_1|
 
.. |fig11_1| image:: ../_images/11/fig11_1.png
    
   
The commands assigned to these blocks can only be executed by sprites. The stage is motionless, which is why it cannot execute motion commands. There are 18 blocks in the group *Motion*, one more than in the version Scratch 2.0. The block |glide_to| was added.  

To make them easier to use, blocks that perform similar functions stand close together and form subgroups. The functions of the subgroups are the following:

1.  moving the sprite in a straight line or in a circle,

2.  moving the sprite to a specified position,

3.  pointing the sprite toward something,

4.  moving the sprite by changing its coordinates,

5.  keeping the sprite within the boundaries of the stage,

6.  setting the sprites rotation style,

7.  storing the current coordinates of the sprite.

Blocks belonging to the first six groups are stack blocks, while the seventh group represents reporters, whose function is to store data. They cannot stand on their own; they are inserted into the input fields of other blocks, thus specifying their actions. 

The blocks from the first group perform relative motion, movement in relation to the current position and direction. Unlike these blocks, the ones from the second group move the sprite to a specified point on the stage, regardless of its current position. This type of motion is called absolute motion. 

Several types of data can be entered into the input fields of motion blocks: values of destination coordinates, rotation angle, number of steps, or duration of movement. One step corresponds to one pixel. The time is expressed in seconds, and angles in degrees.   

In some of the blocks, the destination is chosen from the block's drop-down list. This can be the mouse-pointer, some other sprite participating in the project, as well a point whose coordinates are generated randomly. 

The block |rotation_style| has three rotation style options: *all around*, *left-right* and *don't rotate*. The first option means that the sprite can face any of the 360 degrees. *Left-right* means that the sprite can only face left or right, and any other direction is disabled. The last option means that the sprite always faces right. 

The blocks from the group *Motion* are elaborated in lesson 2 of this practicum. 

.....

Looks Blocks
~~~~~~~~~~~~~~~

.. sidebar:: |looks_blocks| Looks
    
   |fig11_2|
 
.. |fig11_2| image:: ../_images/11/fig11_2.png

The blocks from this group control the appearance of sprites. Seven out of 21 blocks from this group control the appearance of the stage. 
Twenty blocks are visible when the sprite is in focus and three block subgroups when the stage is in focus. The block |switch_backdrop_wait|, which enables the backdrop to change and wait until that happens can be seen only when the stage is active (it is not visible when the sprite is in focus). The remaining blocks that can be attached to the stage can also be seen in this case. The functions of the subgroups are as follows:

1. displaying what the sprite is saying of thinking,

2. changing the costume of the sprite and the backdrop of the stage,

3. changing the size of the sprite,

4. working with graphic effects that can be attached to sprites and the stage,

5. showing or hiding the sprite,

6. putting the sprite in the specified layer of the image,

7. reporters that indicate the current costume and size of the sprite, as well as the current backdrop of the stage. 

Graphic effects, which can be added to the sprite, are: 

.. hlist::
    :columns: 1

    * color - changes the color of the sprite,
    * fisheye - gives the impression of a sprite being seen through a wide-angle lens,
    * whirl - twists the sprite around its center point, 
    * pixelate - pixelates the sprite, 
    * mosaic - creates multiple smaller images of the sprite, 
    * brightness - changes the brightness of the sprite, and 
    * ghost - changes the transparency of the sprite. 


Changing the color, for example, can give the illusion that the sprite is expressing emotions or flashing, it may look like a completely new thing appeared. If you use color change with the ``stamp`` command, you can make attractive patterns, for example, a rainbow. 

By using the fisheye effect, you can give an illusion that the sprite is moving toward or away from the screen, becoming fatter, and the like. It can be used as a transition between costumes. 

The whirl effect can symbolize time travel, teleportation, vertigo, nausea.  

The pixelation effect makes sprites look like they did in the first versions of computer games, when the monitors had low resolution; it can also be used to censor or block out the sprite on the stage. 

The mosaic effect is used for multiplying sprites without cloning.

By changing the brightness of the sprite, it can give the impression of glowing, or it can become darker, and the ghost effect can make the sprite invisible for the user, but other sprites can still detect it on the stage. 

Blocks |goto_layer| and |go_layers| are different from blocks that performed similar functions in the previous version of Scratch.

When the stage is in focus, you can see 8 blocks divided into 3 subgroups: for changing the backdrop, for setting graphic effects for the backdrop and the reporter that indicates the current backdrop. The backdrop ``Backdrop Name``, which existed in the version Scratch 2.0, is not included in the new version.

The blocks from the group *Looks* are elaborated in lesson 3 of this practicum.

.....

Sound Blocks
~~~~~~~~~~~~~

.. sidebar:: |sound_blocks| Sound 
    
   |fig11_3|
 
.. |fig11_3| image:: ../_images/11/fig11_3.png

Two types of sounds can be used in projects: sounds and notes. The blocks from this group can be used for working with sounds, and the blocks from the extension *Music* for working with notes. Sounds are accessible only by importing, recording, or from a built-in library of sounds. They are played using the sound blocks, which control the volume, tempo and more. The *Sound* group of blocks has been modified significantly, compared to how it was organized in Scratch 2.0 version. Some of the blocks from this group were moved to the extension *Music*. The group *Sound* has 9 blocks, which are divided into 3 subgroups. They can be applied to both sprites and the background. 

The functions of the subgroups are the following:

1. starting, stopping and playing sounds,

2. applying sound effects,

3. controlling the volume.

**Starting, Stopping and Playing Sounds**

The block |play_until| plays a specific sound, pausing the script until it is finished. Unlike this block, the block |start_sound| plays a sound without pausing the script. This is why the block ``start sound`` is usually used to announce an action, inform a sprite that a goal has been reached, or highlight certain events.

On the other hand, the blocks ``play until`` is usually used to play the "background music". This block is placed into the block ``forever`` and the appropriate music is played during the whole running of the program. It can also be used for pausing the running of the script instead of the control block ``wait``.

The block ``stop sounds`` will stop all sounds that are currently being played - of all sprites and the stage. For example, if the project offers the option of music, this block is used to turn off the music. It is also common for all sounds to be stopped before the project moves on to the next scene, and the like. 

**Applying Sound Effects**

Blocks that set and change sound effects were introduced in Scratch 3.0. Although the new sound editor provides more sound effects (see below in the sound editor section), the blocks support only two: setting and changing the pitch, and shifting the audio toward left or right.

**Volume Control**

These blocks affect only the sprite (or backdrop) to which they are assigned. For example, clicking on the sprite can turn the volume down if the sprite is getting smaller, thus appearing as if the sprite is getting further away from the user. Also, if blocks from the *Music* extension are used, some parts of the composition may be heard louder and others quieter. 

Eight of these blocks are stack blocks, and one is a reporter block, which stores the information on the volume of the sound.

.....

Event Blocks
~~~~~~~~~~~~~

.. sidebar:: |events_blocks| Events
    
   |fig11_4|
 
.. |fig11_4| image:: ../_images/11/fig11_4.png

The blocks in this group are used to trigger the running of the script and send and receive messages. There are 9 blocks in this group and they are divided into 3 subgroups. Since in this version of Scratch the video sensing has been moved to the extensions part, it has been removed from the drop-down menu of the block |when_greater|.

The functions of the subgroups are the following:

1. triggering scripts with a specific activity performed by the user, 

2. triggering scripts when a specific condition was fulfilled during the running of the project,

3. enabling the broadcasting and receipt of messages.

**Triggering of scripts with activities performed by the user**

The user can start the running of the project by clicking the button |g_flag|, one of the sprites participating in the project, the backdrop or by pressing one of the keyboard keys. The project is usually triggered when the green flag is clicked, this is when all scripts, which start with this block, will be activated. These are scripts that perform various initializations, and then hand over the management to other scripts. For example, they delete all list elements, reset variables, set scenes by showing or hiding sprites and by changing their costumes, delete anything drawn on the stage, start the background music, etc. While it is entirely possible to create projects without using this block, it is not recommended. The only way a project could be started without using this block would be to activate scripts that start with some other block from this subgroup. In this case, the project would only last until the scripts that depend on the initial scripts were completed.

Note. The block |clicked_stage| is visible only when the stage is in focus.

**Triggering scripts when a specific condition was fulfilled during the running of the project**

Some of the events that can trigger the running of scripts starting with one of the blocks from this group are changing of the backdrop, expiration of a specific period of time, or increasing the volume beyond a certain level.

**Broadcasting and receipt of messages**

Broadcasting of messages is the main mechanism for coordinating the behavior of sprites participating in a project, and it can also be used for the realization of procedures. Broadcasting is used for calling scripts that should be activated when certain conditions are met. The scripts that start with the block |when_receive| will be called after the specified message has been broadcast. If the same message is broadcast while the script is still running, the current running will be stopped, and the script will start running again from the beginning. Therefore, if we put the block, which broadcasts the message to which the script is responding, into the script that starts with the block ``when receive``, we have a situation where the script is calling itself. This is called **recursion**, and it can be used for creating fractals, forever loops, and the like.

.....

Control Blocks
~~~~~~~~~~~~~~~~

.. sidebar:: |control_blocks| Control
    
   |fig11_5|
 
.. |fig11_5| image:: ../_images/11/fig11_5.png

The blocks from this group control the running of scripts. They enable branching, repetition, and working with sprite clones, and they can stop the running of scripts. There are 11 blocks in total, one is a starting (hat) block, two are cap blocks, three are stack blocks, five are C-blocks, and the ``if then else`` is an E-shaped block. They are divided into five subgroups, whose functions are the following:

1. block for waiting (pausing the script),

2. repetition blocks,

3. blocks with branches, 

4. block for conditional repetitions,

5. block for stopping the script,

6. blocks used for working with clones.

The functions of these blocks are elaborated in lessons 5, 6 and 7 of this practicum.

**Working with clones**

Cloning is a feature that allows the sprite to create a copy of itself while the project is running. Each clone (copy) has the same costumes, sounds and scripts as the original, but it is otherwise independent. Cloning is different form stamping because clones are individual sprites that can run scripts and behave according to those scripts. They are also different from the sprites created with the duplication option because the ordinary duplicates are permanent and appear in the sprite list, whereas clones do not, and they disappear when the project is finished. 

Cloning is used whenever a project has similar sprites doing similar things. Since clones are made by the project, and not by the user, cloning liberates the user from making the same changes to each of the many sprites. For example, cloning can be used for creating multiple friend and enemy sprites in games, as well as for special effects like fireworks and snow.  

Clones usually perform an action when created. The block |when_clone| triggers the script, which starts running when a clone is created. Multiple scripts starting with this block can be added to the same sprite, and they will all run simultaneously when a clone is created. The script itself can be running on multiple clones at once. Some of the actions that this block can perform include putting the clone in a random position, moving the clone until it collides with another sprite. 

.....

Sensing Blocks
~~~~~~~~~~~~~~~

.. sidebar:: |sensing_blocks| Sensing
    
   |fig11_6|
 
.. |fig11_6| image:: ../_images/11/fig11_6.png

This group is made up of blocks that allow the project to accept input from different devices, much like how the human senses collect information from their environment.
There are 18 blocks in the group *Sensing*. Three blocks, which were in the Scratch 2.0 version and which referred to video editing and monitoring movement registered by a video, are no longer included, but the block |set_drag| was added. This block regulates whether a full-screen sprite can be dragged or not, which was previously adjusted in the sprite's information. The blocks related to video detection have been moved to the corresponding extension.  

These blocks are divided into 6 subgroups with the following functions:

1.  storing information on the distance of the sprite in relation to the mouse-pointer or other objects,

2.  entering input data from the keyboard,

3.  storing information on the current operations of the mouse-pointer and the keyboard,

4.  storing the current value of the loudness of the sound,

5.  working with a timer,

6.  storing parameters of sprites and the stage,

7.  storing information on the current time and the user.

Only three blocks from this group can stand on their own, the rest of them are function blocks. Therefore, the blocks from the first group are inserted into control blocks, which should enable the execution of different activities depending on the position of the sprite. The blocks of the second group correspond to the information that a person collects with the sense of touch, and the third group corresponds to the information that is collected by the sense of hearing. The timer can be used to limit the playing time in a game or the time it takes to complete a test task. The block that stores the parameters of sprites and the stage can provide a lot of data on all of the objects, which participate in the project. Information that a person would collect through the sense of sight, and a computer with a video camera, can be used if the extension *Video Sensing* is added to the project.

We have elaborated the functions of most blocks in this group through the examples in the previous lessons. Here we will just mention the functions of logical blocks and current time reporters.

**Logical Blocks**

There are 5 logical blocks in this group. Each of these blocks can return only one out of two values: true or false, depending on whether the condition was fulfilled or not. Logical blocks are placed in the input fields of the hexagonal shape of the control blocks.

**Current time and user information**

The reporter block |time_unit| can give the following information on the current time. 

.. image:: ../_images/11/fig11_6b.png
     :width: 200px   
     :align: center

.....

Operators Blocks
~~~~~~~~~~~~~~~~~

.. sidebar:: |operator_blocks| Operators
    
   |fig11_7|
 
.. |fig11_7| image:: ../_images/11/fig11_7.png

In the group *Operators* there are no independent blocks, which would correspond to language commands. All blocks are function blocks, i.e. they store the values of number, string or logical expressions and they are inserted into appropriate input fields of independent blocks or other function blocks. The block |text_contains| is a new block in this group, which returns the values *true* or *false* depending on whether the string contains the given character or not. 

There are 18 blocks in the group *Operators* - 11 reporters and 7 logical (boolean) blocks, which enable the following types of operations:

1.  the basic arithmetic operations – addition, subtraction, multiplication and division,

2.  generating random numbers,

3.  comparisons - greater than, less than, equal to,

4.  constructing complex logical expressions,

5.  operations with strings,

6.  integer operations, 

7.  calculating the value of mathematical functions.

Basic arithmetic operations can be performed with integer and real numbers. Only division by zero (divisor = 0) can lead to problems, because there aren't any numbers that, when multiplied by zero, would give a number other than zero (quotient * divisor = dividend). This is why division by zero should be prevented in programs. We showed how this could be achieved in the project *Young Mathematician* from lesson 7 of this practicum. 

As the result of the division by zero, the Scratch interpreter returns one of the values *Infinity*, *NaN* (not a number) or *-Infinity*, depending on whether the dividend is a positive number, zero or a negative number. 

We have explained the use of random numbers, logical expressions, and complex logical expressions formed by the logical operations *and*, *or* and *not* with the examples presented in the previous lessons.

The operations used with strings enable the joining of two strings, selecting characters located in specified positions in the string, determine the length of the string, and check if the string contains the specified character. The operation performed on strings were elaborated in lesson 9 of this practicum.  
 
The integer operations supported in Scratch are the computation of the remainder in the integer division, and the rounding of the numbers.

Mathematical functions that can be selected from the drop-down list of the block |function| are:

.. hlist::
    :columns: 6

    * abs
    * floor
    * ceiling
    * sqrt
    * sin
    * cos
    * tan
    * asin
    * acos
    * atan
    * e^
    * 10^ 

.....

Variable and List Blocks
~~~~~~~~~~~~~~~~~~~~~~~~~

.. sidebar:: |variables_blocks| Variables and Lists
    
   |fig11_8|
 
.. |fig11_8| image:: ../_images/11/fig11_8.png

The functions of the subgroups are the following:

For variables

1. reporters for user's variables,

2. setting and changing the value of a variable,  

3. showing and hiding variable reporters on stage.

For lists

4. reporters for user's lists,

5. adding elements onto the end of the list,

6. operations performed on the list, 

7. returning list information, 

8. showing and hiding list reporters on the stage.

The operations that are supported for working with lists are: 

.. hlist::
    :columns: 1

    * deleting an item from a specified position on the list,
    * deleting all items from a particular list,
    * inserting items into the list at given positions, and  
    * replacing items in specified positions.

The following information can be obtained about the list:

.. hlist::
    :columns: 1

    * which item is in the specified position, 
    * what is the position (on the list) of the specified item, 
    * the length of the list (number of items on the list), and 
    * whether an item is included in a list or not. 

Variable and lists can be global - they can be used by all sprites, or local - they can be used only by one sprite. The variables and lists created for the stage are visible to all sprites. 

Current values of the variables can be followed on the stage via variable monitors. Variable monitors can come in three formats: 

.. hlist::
    :columns: 1
    
    * displaying the value with the name of the variable,
    * large display of the value without the corresponding name of the variable, 
    * display containing a slider bar, which can be used to change the value of the variable.

Variables are elaborated in lesson 7, and lists in lesson 9 of this practicum.
 
.....

My Blocks
~~~~~~~~~~~~

.. sidebar:: |my_blocks| My blocks
    
   |fig11_9|
 
.. |fig11_9| image:: ../_images/11/fig11_9.png

The option for the user to make his/her own blocks and thus implement procedures was first introduced in the Scratch version 2.0. In the new version of Scratch, the color and the shape of user's blocks were changed. 

The define block is the first block that will appear when the user asks to introduce a new block. The actions, which should be performed by this newly introduced block, should be added onto the define block. Then a stack block will appear in the block palette with the name assigned to it in the definition. The new user-defined block can further be used like any other block.    

The new block can have input fields. *Parameters* are inserted into the input field of the definition header. Procedures can have more than one parameter. When the new block is used to call a procedure, in its input fields the user will enter *arguments*. The arguments replace each appearance of the corresponding parameters in the procedure.

The creation and the use of introduced blocks are elaborated in lesson 8 of this practicum.

.....

Blocks of the Pen Extension 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. sidebar:: |pen_extension| Pen
    
   |fig11_10|
 
.. |fig11_10| image:: ../_images/11/fig11_10.png

In Scratch, each sprite can be assigned a position, direction and orientation of movement and it can leave a mark while moving. In doing so, the size, shape and color of the sprite have no effect on the mark left by the sprite drawing with a pen. The sprite can be invisible, or it can consist of a single dot, but this does not affect its drawing. The sprite's ability to leave a mark while moving is based on blocks from this group. Images that are created by sprites are stored as a collection of figures, along with their parameters. Images defined in this manner are called *vector graphics*. 

The blocks in the *Pen* extension are divided into 5 subgroups. Shade pen command from the previous versions has been taken out, and instead of setting pen color by number alone, color is now defined by hue, saturation, and brightness. All blocks belonging to this group are stack blocks.

The functions of the subgroups are:

1.  deleting everything drawn (removing all pen marks from the stage),

2.  stamping the sprite,

3.  putting the pen up or down,

4.  setting and changing pen attributes,

5.  setting and changing pen size (thickness).

The graphical editor in this version of Scratch is working with the so-called HSB (Hue, Saturation, Brightness) color model. This means that the color is built with 3 components: Hue, Saturation and Brightness. The color shade indicates the color number in the spectral palette, that is, the color itself. It is described in a color circle in which the 0° angle represents the color red (color number is zero), and the 180° angle represents the blue-green color called cyan (color number 100). The saturation refers to the intensity of the color - the higher the saturation, the purer the color. The saturation can be from 0 to 100%, with the 0% intensity representing white and the 100% intensity pure color. The brightness of the color depends on the amount of the color black mixed in with the observed color.  

.....

The Blocks from the Text to Speech and the Translate Extensions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. sidebar:: |voices_extension| Text to Speech and |translate_extension| Translate
    
   |fig11_11|
 
.. |fig11_11| image:: ../_images/11/fig11_11.png

**Text to Speech Extension**

This extension can be used only if the computer is connected to the Internet |requires|, because it uses the Amazon Web Services.

When you choose |voices_extension| from the group *Extensions*, three new blocks will appear in the block palette. They allow the sprite to say the text inserted into the input field of the first block, in the language set by the user with the third block from this group. The user can also set the voice, which will actually speak the text: female (soprano or alto) or male (tenor or bass). This is set by another block from this group.   

**Extension Translate**

This extension can only be used if the computer is connected to the Internet |requires|, because it uses Google. 

When you choose the |translate_extension| from *Extensions*, two new blocks appear in the block palette. They allow the text written in one language to be translated into another language. The block |language| shows which language is set in Scratch. Text written in the current language in the first input field of the block |translate_to| is translated into the language selected from the drop-down list of the second input field. If the translation block is placed in the input field of the block ``say`` or ``think``, the user can see the translation.  

Using the built-in graphics (paint) editor
--------------------------------------------

Scratch has a built-in paint editor that you can use to create and modify sprites, costumes, and backdrops. This editor supports two different drawing modes: raster (bitmap) and vector. 

.. infonote:: 

  Computers can store images in two ways: raster and vector.
  
  In **raster graphics** the image is stored as a rectangular grid of pixels - bitmap. The bitmap is technically determined by the width and height of the sprite in pixels and the number of bits needed to store the color of the pixels. For example, if we have 16 colors, 4 bits per pixel are required for storing its color. The raster graphics is dependent on the resolution. Raster images cannot be enlarged without losing the image quality.

  This disadvantage is overcome by the application of the **vector graphics**, which stores an image as a collection of figures together with its data (parameters) that defines how the figure will be drawn and where it will be located. The turtle graphics is an example of the vector graphics.

  The following figure shows an enlarged image of a line drawn in these two ways.

  .. image:: ../_images/11/fig11_12.png
     :width: 210px   
     :align: center

User Interface
~~~~~~~~~~~~~~~

The following figure shows the layout of the built-in paint editor in vector and raster mode. 

.. image:: ../_images/11/fig11_13.png
     :width: 1200px   
     :align: center

.. sidebar:: New costumes
    
   |novi|
 
.. |novi| image:: ../_images/11/fig11_14.png

**Costume Area**

To the left is the costume area (1) with icons for each costume and the sequence number of the costume. At the bottom of the costume area is a button for creating new costumes. To edit different costumes in the paint editor, simply click on the icon of the desired costume and the corresponding image will appear in the editing area - drawing area or canvas (7).

You can add a new costume (or backdrop) by hovering over the button |b_sprite| located at the bottom of this area with the mouse-pointer and choosing one of the options that will appear. You can choose a costume from the costumes library, draw your own, download an image file from your computer, take a picture, or choose a "surprise costume", which is randomly selected from the costumes library. 

Note. The costumes library contains individual costumes of all sprites found in the sprites library.

.. sidebar:: Changing the mode of operation 
    
   |vector_bmp|
   
   |bmp_vector|
 

**Converting the vector mode to raster mode and vice versa**

Below the lower left corner of the drawing area is the button (2) that switches the editor from one mode to another. The tools specific to the particular mode can be found on the left side of the screen next to the drawing area, in our figure the vector mode is marked with (5) and raster (bitmap) mode with (6). The options can be seen above the drawing area (canvas). Some of them are common to both modes of operation, in the figure, these options are framed with red rectangles (3), and some of them apply only to the vector mode, these are framed with grey rectangles (4). 

Common options
~~~~~~~~~~~~~~~

These options are located above the drawing area.

.. sidebar::  Changing the color
    
   |promena_boje|
 
.. |promena_boje| image:: ../_images/11/fig11_15.png

|fill| **Changing the Color**

Clicking on the input field of the block that is used to set the color will open a drop-down menu containing sliders: color, saturation, and brightness and below them an eyedropper tool (pipette) for sampling color. You can set the color you want by moving the slider or clicking the eyedropper tool.

Moving the *color* slider changes the hue of the color (for example, from red to blue). This tool is the most commonly used because it has the largest difference between colors. 
Moving the slider *saturation* changes the intensity of the color: the saturation 100 is the selected color, 50 - is a lighter color, and 0 - is completely white. 
Moving the slider *brightness* changes how dark the color is: the brightness 0 is completely black, while 100 is the selected color.

When you click on the eyedropper tool, a magnifying glass appears with a circle in the center. 
To select the desired color, you need to position the center of the magnifying glass above the part of the drawing area on which that color is located and click. 

There are four options above the three sliders. These enable different ways of filling in an area with color. An area can be filled in evenly with a solid color, or as a gradient, with different shades of a color. If you click one of the options other than the solid color option, two selected colors will appear: |swap|. By clicking on the first or the second color you can set them. Clicking *swap* between the two colors changes their order. The fill options are: solid color, vertical gradient, horizontal gradient or circle gradient. 

|size| **Changing Pen Size**

There is an input field to select the pen size (thickness). You can type in the size or use the arrows on the side to change it. The higher the number, the thicker the line.

|name| **Naming Costumes**

The name of the costume is important for the organization and sometimes also for the programming of the project. Since each costume is assigned its own sequence number, it is not recommended to name the costumes by only using numbers without any other characters. To name a costume, you should click on the text bar at the upper left corner of the paint editor and enter the new name.  

|copy| **Copying and** |paste| **Pasting** 

The second row of options includes copy and paste buttons. The copy option copies the selected area, while the paste puts it somewhere else. You can also use the keyboard shortcuts: Ctrl+C to copy and Ctrl+V to paste. First, select the rectangular area you want to copy and then drag it to where you want to place the copy.

|redo| **Undo and Redo**

On the right, next to the costume name, there are two buttons called undo and redo. These buttons allow you to undo the last action or repeat the action you previously undid. The redo button cannot be used unless the undo button has been used. If you exit the paint editor, everything you have done in it will become permanent and it can only be undone manually. The keyboard shortcut for the undo option is Ctrl+Z.


|flip_h| **Horizontal**  |flip_v| **and Vertical Flipping**

When you select an object, there is the option to flip it horizontally or vertically. In the second line of options, there are two buttons with two arrows each pointing to a dotted line. The one on the left flips the selected object horizontally, and the one on the right vertically.

Vector Editor Options
~~~~~~~~~~~~~~~~~~~~~~

These options are available only when the graphics editor is in vector mode and do not appear when it is in raster mode.

**Precise Object Movement**

When an object is selected in the vector editor, the arrow keys can be used to move it precisely one pixel. In raster editor, the user can also use the arrow keys to move selected areas. This option can be useful if you want to make a precise drawing or align different objects.

.. sidebar::  Changing the Outline
    
   |promena_konture|
 
.. |promena_konture| image:: ../_images/11/fig11_16.png

|outline| **Outlines**

On the right of the option used for setting the color, there is a drop-down menu that allows the user to change outlines of objects. This drop-down menu has three sliders, but unlike the color-setting menu, here the user does not have the option to mix two different colors. On the right, next to that drop-down menu, is an input field where the user can select the thickness of the outline. You can type in a number or use the arrows to change it.  

**Layering the Image**

We can use the following analogy to explain how sprites are presented on stage. Imagine that each sprite is drawn on a separate sheet of transparent foil and that all sheets are stacked over the one on which the background is painted. In Scratch, these transparent sheets of foil correspond to **layers**. Every time a sprite moves, it will cover the images drawn on the layers beneath. 

At the upper right part of the paint editor, there are four buttons, which allow you to move objects through different layers:  

.. hlist::
    :columns: 1
    
    * |v_forward| moves the object one layer forward (in front of the current one),
    * |v_front| moves the object all the way in front,
    * |v_backward| moves the object one layer backward (behind the current one),
    * |v_back| moves the object all the way back.

|v_group| **Grouping** |v_Ungroup| **and Ungrouping**

This option is used to group multiple objects into one whole. When there are many objects that you need to move at once, it can be useful to group them. This way, they can all be moved or deleted at the same time. To select objects, click and drag the mouse-pointer over the desired objects (or hold down the Shift key on the keyboard and click on each object), and then click the grouping option. From this point on, all objects will be treated as a single object. 

The ungrouping option does the opposite - the selected group can be broken down into smaller parts. This button will become visible once you have selected a group of objects and it will allow you to ungroup them.   

|v_curved| **Curved** |v_pointed| **or Pointed**

When using the reshape tool, there are two options to the right of the outlines, which allow you to make the splines either curved, like an ellipse, or pointed, like a rectangle. This is useful when creating shapes with both curved and pointed edges. If more than one point is selected (hold the shift key and click on more than one), the specified change will be applied to all selected points.

Working in the Raster Mode
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. sidebar:: Raster Tools

 |rasterski|

.. |rasterski| image:: ../_images/11/fig11_17.png
  
|r_brush| **Free-hand Drawing**

You can set the color and the size (thickness) of the paintbrush with the appropriate options. Use the undo and redo options if you make a mistake. You can also use the eraser for correcting mistakes. 

|r_line| **Drawing a Straight line**

You can change the line thickness with the appropriate option. Press Shift and drag to draw horizontal or vertical lines. 

|r_circle| **Drawing an Ellipse**

You can draw a hollow (outlined) or filled (with color) ellipse. Press Shift and drag to draw a circle. With the appropriate options, you can select the fill style and change the thickness of the outline.

|r_rectan| **Drawing a Rectangle**

You can draw a hollow (outlined) or filled (with color) rectangle. Press Shift and drag to draw a rectangle. With the appropriate options, you can select the fill style and change the thickness of the outline.

.. sidebar:: Text

 |tekst|

.. |tekst| image:: ../_images/11/fig11_18.png

|r_text| **Writing Text**

Click anywhere on the drawing area (canvas) and when the cursor appears, type the desired text. Then click outside of the text area. The select tool automatically selects the text, so you can change its size and orientation. You can use the measurement box that appears on the outer edge of the selection box (circles and arrows around the text) to resize and change the orientation of the text.

|r_fill|  **Filling closed areas with color**
 
You can fill the area evenly with one color or as a gradient, with shades of colors using the appropriate fill option.

|r_eraser| **Free-hand Eraser Tool**

You can set the size of the eraser by using the appropriate option. The erased areas become transparent.

|r_select| **Selecting a Rectangle-shaped Area**

The selected area can be:

1.  dragged to a new location,

2.  made larger, made smaller, or rotated,

3. erased by pressing the Del key on the keyboard.

Working in the Vector Mode
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. sidebar:: Vector Tools

 |vektorski|

.. |vektorski| image:: ../_images/11/fig11_19.png

|v_select| **Selecting an Object**

This tool is used for moving, erasing, resizing and rotating objects. When you click on an object, a frame will appear around it |izbor_objekta|, which indicates that the object is selected.

.. |izbor_objekta| image:: ../_images/11/fig11_20.png

If you want to select multiple objects at once, click the left mouse button and drag the mouse over the desired object or hold the Shift key and click on each object you wish to select at the same time. 
When you move the cursor near the center of the object, it changes its shape and becomes a hand, which means that you can move the object around on the canvas. The object can also be moved with the keyboard arrow keys. 
The selected object can be deleted by pressing the Del key. Objects can be resized with the measurement boxes that appear on the outer edge of the selection box.
To rotate an object, grasp and drag the rotation arrows.

|v_reshape| **Reshaping an Object**

Click on the object you wish to reshape and a set of control points will appear on the perimeter of the object, as shown in the figure (1). Click on one of the control points and drag (2). By clicking on the outline of the object you can create other control points (3).You can delete a control point by bringing the cursor to it (4). The selected point will change color and then you should click on it (5). The buttons |v_curved| and |v_pointed|, which appear in the options, allow you to curve or point the outline of the object.    

.. image:: ../_images/11/fig11_21.png
   :width: 680px   
   :align: center

|v_brush| **Free-hand Drawing**

This tool is similar to the corresponding tool in raster mode. Hold the mouse cursor and move it to draw a curved line. Instead of pixels, the spline here is defined by a set of control points. You can change the appearance of the line with the tool *Reshape*.

|v_eraser| **Eraser**

This tool is similar to the corresponding tool in raster mode.

|v_fill| **Filling closed areas with color or coloring the outline of an object**

The paint bucket tool in vector mode works differently than in raster mode, where the tool fills in any selected closed area. Vector mode bucket only works with vector objects. After selecting this tool, you can change the color or the outline color of an object by clicking on it.

|v_text| **Writing Text**

Click on the tool and then anywhere on the canvas; when a cursor appears, begin typing the desired text. Once you have finished, click anywhere outside of the text area. The tool *Select* will automatically select the text, so you can change its size and orientation. Unlike the text in the raster mode, the text created in vector mode can be edited at any time, even after exiting the paint editor. To be able to modify its contents, you only need to select the text.

|v_line| **Drawing a Straight Line**

The line is defined by two control points at both ends. To draw a line, click and hold the mouse where you want the line to start, and drag to draw the line to the end point. To draw a horizontal or vertical line, hold down the Shift key while dragging the mouse.

To draw a curved line, you must first draw a straight line, then select the tool *Reshape*, press Shift and click anywhere on the line to create a new point and then drag the new control point. This is a way to form a curved line.

|v_circle| **Drawing an Ellipse**

Use this tool if you want to draw an ellipse in the color chosen for drawing. Click to highlight the top left corner, then drag (hold the shift key while drawing with the ellipse tool) until you get the size you want. You can change the fill style (filled or blank) and line thickness by using the buttons in the options area. The created ellipse has 4 evenly spaced control points.

|v_rectan| **Drawing a Rectangle**

Use this tool if you want to draw a rectangle in the color chosen for drawing. Click to highlight the top left corner, then drag (hold the shift key while drawing with the rectangle tool) until you get the size you want. You can change the fill style (filled or blank) and line thickness by using the buttons in the options area. The created rectangle has 4 control points, one on each end.

Using the Built-in Sound Editor
--------------------------------

The sound editor allows users to edit and remix the sounds. In music, the term *remix* is used to refer to a new, modified version of a music composition.

The User Interface
~~~~~~~~~~~~~~~~~~~~

The sound editor window is divided into two areas: the sound list (1) and the editing area (2).

.. image:: ../_images/11/fig11_22.png
   :width: 880px   
   :align: center

.. sidebar:: New Sound

 |novi_zvuk|

.. |novi_zvuk| image:: ../_images/11/fig11_23.png

**Sound List**

The sound list is located on the left side of the window and it is used for selecting sounds, which will be edited in the editing area. You select a sound by clicking on it. A thick blue outline will appear around the icon of the chosen sound, similar to the one around the active sprite in the sprite list. An "x" appears in the upper left corner of the active sprite, which allows it to be deleted.  

At the bottom of the area, there is a button |b_sound|, which enables the introduction of new sounds.

**Editing Area** 

The editing area has a bar on top (3), a graphical representation of a sound in the middle (4) and a bar on the bottom (5), which contains 7 tools. 

In the top bar are the tools that edit the sound, but do not add any effects. These are:

.. hlist::
    :columns: 1
    
    * a name field for the sound,
    * the undo and redo buttons, and
    * the button |trim|, which deletes selected parts of the sound.

In the bottom bar are the tools, which make special effects while the sound is playing:

.. hlist::
    :columns: 1

    * |faster| - faster,
    * |slower| - slower,
    * |echo| - echo,
    * |robot| - robot,
    * |louder| - louder,
    * |softer| - softer and
    * |reverse| - reverse, makes the sound run backward. 
    
Making the sound faster or slower is achieved by playing the higher or lower note instead of the actual one. The echo effect is achieved by re-playing the sound after 0.15 seconds.




