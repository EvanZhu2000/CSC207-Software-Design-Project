# CSC207-Software-Design-Project
Simple mobile game design using android studio with classmates.





THANK YOU FOR CHOOSING TO PLAY CSC207 SIMULATOR.

This is a fun application that consists of three mini games.

-----BACKGROUND STORY------

You are a student of CSC207 at the
University of Toronto. Will you survive the harsh challenges of university life? Or will you fall
into the traps of useless textbooks, unhelpful teachers, and inescapable nightmare dungeons?

Your adventure will start from now on, be the best student of CSC207!


-----INSTALLATION AND REQUIREMENTS-----
When cloning:
	Make sure the project location ends in phase2/CSC207Simulator
	Select Android API29 Platform when prompted to choose the project SDK

Chose Pixel 3 API 28 as the device to run the application on.

If you wish to run this on an older version of Android, in build.gradle, you may change
minSdkVersion under defaultConfig from 28 to the SDK version of your device.

Please confirm that the build.grade's dependencies are as follows:

dependencies {
    implementation fileTree(dir: 'libs', include: ['*.jar'])
    implementation 'androidx.appcompat:appcompat:1.1.0'
    implementation 'androidx.constraintlayout:constraintlayout:1.1.3'
    testImplementation 'junit:junit:4.12'
    androidTestImplementation 'androidx.test.ext:junit:1.1.0'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.2.0'
    implementation 'androidx.gridlayout:gridlayout:1.0.0'
    implementation 'com.google.code.gson:gson:2.8.6'
}


-----GAME DESCRIPTIONS-----
This application has the capability for creating an account. Account information is stored locally
on the device.

There are three customizable aspects: 
	The language can be changed to English or Chinese
	The theme can be changed to a Light or Dark theme
	The third game has a choice between beginner, intermediate, and hardcore

Three statistics will be tracked for each player:
	Knowledge - the amount of knowledge the player has gained through each game
	Performance Score - calculated based on how well the player plays each game
	Score - calculated differently in each game based on different aspects
In addition to these, you can also view your highest score.

Each game contains a hidden action where you can gain more knowledge. See if you can find the hidden
actions for all three games!

General descriptions of the mini games:

	Game One: You have 60 seconds to click on as many books as possible. Each book will have a
	number of times you must click on in order to open(ie. complete reading) the book. When a book
	has been opened, you will gain some knowledge. Beware, some books may not offer you what
	you desire, and will reduce your knowledge!

	Game Two: 5 teachers are displayed on the screen that you may attempt to trade with. When you
	choose a teacher guess 0 or 1, (0 and 1 represent whether this is a ta or professor).
	If your guess is correct, the teacher will reveal if they are a professor or a TA and
	let you trade knowledge with them, otherwise they will be disappointed and will leave :(.
	If the teacher lets you trade with them, you may then input the amount of knowledge you with to
	share with them. If the teacher is satisfied with the knowledge you have given them, they will
	return your knowledge, with additional knowledge to add to your wonderful mind. However, if the
	knowledge you give is too much the teacher may not be able to give you any knowledge at all.

	Game Three: You have fallen asleep while studying, and awake in a dungeon of knowledge! There
	are hidden treasure chests containing knowledge. However, you must use equipment to uncover the
	treasure chests of knowledge, and you must guess where the chest is hidden in order to
	successfully uncover the chest. If clicking on a tile reveals a card, it displays a number on
	how close a chest may be. To make a guess on where a chest is located, click and hold a tile to
	use an equipment. If a tile clicked shows a chest, it means you have failed to guess where the
	chest is and you will not gain any knowledge from it. You have a limited amount of equipment,
	so be tactful!

After the game there will be a scoreboard displaying the ranking of the players, and you can choose
to rank them by any of the 3 statistics. (Of course as the game is stored inside your device, the
ranking is only for the accounts you create XD)

NOTED! The app will automatically save the setup preferences and your score, knowledge, performance
score AFTER you finish each game, so beware to finish the game so as to get your statistics saved.


-----ANY OTHER INFORMATION-----
The structure of the game is basically completed in phase 1. In phase 2 we concentrate on improving
our architecture, fixing the bugs left in phase 1 and modifying the user interface. Specifically,
all of our packages

We are still fixing the uml diagram and it will be presented in the presentation:)


-----REFERENCES FOR IMAGES-----
1)"BookIconTemplate" by smirlianos licenced CC0:
    https://opengameart.org/content/book-icon-photoshop-template
2)"Paper Popup Backgrounds" by ztn licenced CC-BY 3.0
    https://opengameart.org/content/paper-popup-backgrounds
3)"Teacher" by prizzy96 licenced CC-BY-SA 3.0:
    https://opengameart.org/content/teacher
4) Game icons used in game three by
    game-icons.net https://game-icons.net/
