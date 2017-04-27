# Intro to Command Line - Full Lecture

## Objective
***Students will be able to navigate their system's file structure using the command line in
terminal.***

## SWABTS

+ CLI ‐ Understand and explain what terminal is and why we use it.
+ CLI ‐ Navigate through directories using relative and absolute paths*
+ CLI ‐ use the `cd` command to move up and down directories
+ CLI ‐ Use the `ls` keyword to list items in a directory
+ CLI ‐ Remove a file and a directory by using `rm` and `rm ‐rf` keywords
+ CLI ‐ move files and directories using the `mv` command

## Motivation
Back in the day ('80s') computers only had a terminal to control them. (Show a picture). No mouse, no icons, no desktop. Just a blinking green cursor. You had to control your entire computer like that.

Later on, GUIs were created to make computers more accessible.

+ Developers continue to use the terminal instead of the GUI because it makes you faster, more in control, you understand what's happening under the hood. If you're a developer, time is money (and your time is expensive).
+ Understanding the terminal is like being Neo from the matrix- you can see the secret hidden files on your computer. This is industry practice.

## Lesson Plan 

+ We're going to learn about the command line by planning for a trip. In Cloud9, your terminal is located at the bottom of the screen. In your terminal, type `pwd`. (stop and have all students do this) `pwd` stands for print working directory. It will tell you where you are currently "standing" in terms of directories. A directory is just a fancy shmancy word for a folder.

+ A directory can contain one of two things - files or other directories. The directories on your computer are nested inside of each other, like a Russian doll or a tree structure. (draw the tree structure out as you build it)

+ When you open your terminal you'll see a tilde: `~/workspace`. The workspace directory is inside of '~', which stands for your root directory. For cloud9, you'll always want to be inside of the 'workspace' directory. 

+ Let's check what directories are within the directory where you are standing by using `ls`, which stands for list (have students do this).

+ Create a new directory called "development", using `mkdir`. This stands for make directory. (have students do this) `mkdir development`

+ Change directories using `cd` command. `cd` into development. (stop and have all students do this) `cd development`

+ To get some practice, we're going to make a new directory on for a trip. make a new directory called `trip` by using `mkdir trip`. Check and see that the directory was made by using ls. (stop and have all students do this)

+ Create directories for countries within the trip directory

```
mkdir egypt
cd egypt
```

+ Create directories for cities within the countries (stop and have all students create countries and cities)

```
mkdir cairo
cd cairo
```

+ Create text files for places you want to visit in the cities directories by using touch:

```
touch pyramids.txt
```

+ Open the file using the file browser on the left navigation bar. (pause and have students create files with text.)

+ remove a file that you no longer want using rm (I don't want to see eiffel_tower.txt anymore) `rm eiffel_tower.txt`

+ remove an entire directory using `rm -rf` (remove paris directory) `rm -rf paris`

+ Accidentally place a file in the wrong directory so we need to move it. (`washington_monument.txt` in `new_york` directory needs to be moved to `washington` directory)

+ Practice moving up the tree using .. (`cd ..` moves backwards)

+ Important: directories only know what's directly inside of them. If I'm in Paris, the only things I know are the sights in Paris, I don't know that I'm in France, and I don't know that Rome even exists. You need to move up the tree with .. to access items outside of the directory you're in. 

+ Write out the absolute path of different files and directories. An Absolute path is a path that starts from the root directory. In the case with c9, the root directory is called `~/workspace`. An absolute path to the pyramids file would be: `~/workspace/development/trip/egypt/pyramids.txt`.

+ Write out the relative path to the cities from the trip directory. A relative path changes based on what directory you're in. If you're inside your `development` directory, and you're trying to get to your `pyramids.txt` file, the relative path would be `trip/egypt/pyramids.txt`.

+ It helps to draw out the file structure tree on the board, and use that as a visual to draw out the path.


## Conclusion 

The Command Line is an incredibly valuable tool that lets you manipulate configuration files of your computer. It also lets you navigate your computer much faster than using the Finder. We will also use the command line to run our code, so familiarity with it is very important.

## Hints and Hurdles

+ The [Refrigerator Organization]() lab really hammers home paths. This is an important concept for students as they begin to create HTML/CSS projects and then their sinatra apps at the end of the course. Paths are a complicated concept- let students know its ok if it doesn't make sense right away.

+ Bonus Labs are the Terminus Game and the Command Line Challenge!

+ Helps to have students write out the instructions if they were moving one step at a time `cd code`, `cd labs` and then show them how they can shorten that `cd code/labs`.

