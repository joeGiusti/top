========== ========== ========== ========== ========== ========== ========== ==========
            This section contains random notes and ideas about htis project
========== ========== ========== ========== ========== ========== ========== ==========

When sending the real estate course to the frec to be approved have a comments section agfter each question so they can write exactly what they think ando if anythin needs to be changed


Shout into the void with such intensity that your echoes are felt by postarity;

sigin info
example@example.com
pass1234

==========
random ideas:
mention things in questions that remind reader of things even if they are not the correct answer
ex: a ground lease is often used for farming and can be up to 99 years long so mentioning farming lease or 99 year lease before the correct answer will help to solidify that piece of information
another example: putting an answer choice for a vocab word that is going to be mentioned in the next slide will make it more familiar and more likely to be remembered
use fat dating and dopamine fast as motivational videos
==========

start with index

working on:
different things show when user clicks on class based on if they are the owner of it or not
guided study viewing page
guided study editing page

go thru the home page and understand how it all works
including js and firebase stuff

decide what the desired funciton is
make it happen

layers:
words
transparent torch
background color

=====
user
  attempted modules
    moduleID    
      position: 0
      attempted questions
        questionID
          givenAnswer: 0
          correct: false

classID
  allQuestions
    questionID
      content: "question" 
      answers
        answerID
        correct:true

when clicked view check to see if module is in users attempted modules
if it is load their posiiton and show all tiles up to that one
if not set it to 0
when clicked "got it" show next tile abs increment position it in firebase


maybe just put atart and end times in video for now
ans questions go after that

for dark theme find all elements with class light theme
that will have no attributes so it will be default
add dark theme to those elements
dark theme will change their colors based on what kind of element they are

classes page will have add, browse, create buttons
in rowse it has info like the rating

hover over information icons in tiles area with description of wha it is doing

checkbox to select the correct answer in question tile

question by default asks the last 2 questions as well after the new one
questions by default cover up the last three questions or all
maybe just blur it out somehow or show a dark screen as to avoid disorientation

show password checkbox (show it by default though)

get the script link to work so same code can bo on all pages

landing page can be like firebase landing page
video in back with cards overlay
color image below with diagonal lines and still card overlays

live class chat would be cool
live chat at home page would also be cool

make it so the amount of text doesnt affect the card height

cards 
2
2
2
big
then
3
3
big

view readme in hosted folder

==========
to accomplish:

*search updated
need to save contents from html
right now just saves from array which is not in sync with html input fields

DONE) anonomous login
DONE) sign up
DONE) sign up goes into db
DONE)add to the database
REVISIT WHEN HTTP)google sign in
3) class page that opens when you click a class (and shows modules)
  DONE) make page
  DONE) copy code and take out un-needed
  DONE) load class modules
  4) load class sessions
  4) load class labs
  4) make cards with class data
   ) placeholder is still showing
 DONE) new module button
   DONE) new module modal popup
   DONE) makes new module in db 
   DONE) show new module
      )DELETE MODULE BUTTON
      ) confirmation popup or madal
      ) delete button deletes from databse
      ) removes deleted modulefrom html
  DONE) view module button shows module html
  DONE) edit module button shows edit module html


4) view module page
  DONE) create page html
  DONE) load module info 
   ) show html for info
   ) next button 	
  +) only shows one at a time
  +) saves if the user completed
  +) saves users progress

5) edit module page 
  DONE) load module info
  DONE) show info in tiles
  DONE) add tile button
 DONE) add tile button
  DONE) adding a tile puts it in the array
   DONE) then shows it
   DONE) adding a tile puts it in the db (when click save update)

  DONE) change position button
   DONE) delete tile button
   DONE) deletes in array
   DONE) deletes in db
   DONE) save tiles button
   DONE) when clicked save all new tiles and updates into the databse (update or overite?)
   DONE) autosave
==
Tile Types

  DONE) change tile type dropdown
  DONE) changes type in database
  DONE) adds neccisary sections in database (question will be content, add answers section and add t/f)
  DONE) loads type from database
  DONE) text option works
  3) shows type in dropdown (handle this by changine selected in the html for the other type)

put a background image or color option for the tiles
  2) change html when type changes


1+) create question type
  ) shows this type if type in databse is quesiton
  ) question saves into database
  ) question type loads from databaase
load answers from db into tile
save correct answer change into db

  +) create video type
  ) shows video
    add questin button with time to show (over vid time and it shows at end) also end option
    pause at certain times for questions
    show question at that time
  ) video saves into database
  ) video type loads from databaase


   ) tutorial video

==========
*

1) save function will update the tiles array based on the tiles on the screen before updating or pushing to the db
position up and down will change the position for the tile and the one next to it with a temp tule holder
maybe make them all have the same class of tileDisplay and get elements by class
==========


custom card with background color

loads class modules and other stuff for the class

back button history to home from class page
https://code.google.com/archive/p/reallysimplehistory/
https://stackoverflow.com/questions/1462719/javascript-change-the-function-of-the-browsers-back-button

add moderator button can add people to edit the class (maybe add approval before edit are finalized eventually)
add text button
add question button
ad video button
app that allows to select the class and asks all the quesitons in the class verbally

add tile button between each tile and changes positions accordingly

create class button
users have enrolled classes owned classes, moderating classes (all show)

home button just changes what is showing instead of reloading page to reduce data usage

if start from a real estate school site automatically create account and add real estate class

sidenav responsive for phones
maybe big card for background of sections on home page

show completion percent and test/question score 

more points if the first time answered a particular question correct regardless of what platform answered on
ex: if got wrong in the module but correct in the game get more points in the game than if its a repeat correct
maybe progressively less3 points, then 2 then 1 then 0
but maybe it comes back after a certain amount of time

account page
anonymous user is able to become a perminant user
http://firebase.google.com/docs/auth/web/anonymous-auth

=====
applications:

real estate course
re-create for fake
clep courses
university professors tool (paid by students)
home schooling courses
teaching my self things
turn into real university
=====


quesitons by default ask the last question too
hides the text so you cant just read back (or maybe goes over it)
shows the number of sections completed, score, number left
questions saved in database and 
auto quiz option puts a quiz with all of the questions from before in random order
questions also show up in other places like pvp game and team game
maybe as passwords getting into doors in the labs

point system


more info button for classes in the browse catigory
example: real estate class can have a brief description but in more info it can give
stats about the number of people salaries, time to complete, etc

adding to modules is like tiles
they have an index in the databse
there are arrow buttons that change the index an reload (or just move)
add tile button, then choose drom dropdown the type
tutorial video
start with a text tile
reccomended length, but will let go over
have a study showing the reason for the text length reccomendationthat can be clicked on

add a yoga or stretching lab
add a mem class free in browse

video feed of lecture with question on botom
you answer it in the browser
in the actuall class it shows as the whole screen
put in demo video with side by side screen one showing in the class with the big question
and people on their phones, and next to it someone at home watching the lecture seeing the quesiton
also a class chat

also for demo video: virtual campus 

save button, exit without saving button
on back pressed or on destroy save automatically

dark mode 
saves on profile and in browser

=====
when <module view> or <module edit> are clicked
set currentModuleId
use it to load all tiles from database into an array of tile class instances (similar to load classes info)
show the module edit or view section with display = normal, other displays = none
make tiles into html (depending on view or edit, listed below)

for View:
call refresh function that clears and puts html for each tile in the array (similar to use class id array)
only show the right ones somehow
for edit
call different refresh function that shows tiles in a differnet way
or maybe just have an editing variable that determines if refresh calls a different add html function
also will call differnet add html based on tyle type variable
call firebase update function when edits are made
save button that is a bright color when there are unsaved changes
add tile button creates a tile instance with some values and adds it ot the array
then you can edit the tile
