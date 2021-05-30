# SPACE-DEFENSE

The development of the game consisted of three main milestones with the respective order of priority:

1. Processing game design
2. Arduino architecture
3. Serial connection

Accomplishing the first milestone, therefore, took up the most time. I initially made the game without the Arduino part and included the use of the keyboard to make the development more convenient and seamless. This is because it seemed rather easier for me to replace the keyboard use with the button use through serial communication than leaving numerous chunks blank. I still commented out not all but most of the parts necessary to run the keyboard to play the game. So find parts as shown below and simply uncomment them to use the keyboard instead (apart from the uncommenting you need to do some tweaking into the code of course).

In terms of the code in Processing, I have in total of 4 classes (Player, Laser, Item, and Asteroid). I used polygons instead of images on asteroids for three reasons. First, when I used resized images instead of polygons it made the whole game slow. Second, I thought it would be awkward to recreate the specific movement effect on an image, and the way my code generated different shapes, sizes, trajectories made the game more resourceful. Lastly, employing shapes instead of simply importing images seemed like a bigger challenge to me so I went with it. This is because these polygons have different shapes and vertices and so the collision effect on them required more thinking and effort than on uniform images.

With this problem and user experience in mind, I decided to use push buttons. I also decided to get rid of UP & DOWN buttons because it made physiologically little sense that LEFT & RIGHT & UP & DOWN buttons are all aligned next to each other. So the spaceship was only allowed to move sideways and this was enough. I then added two push buttons – one for shooting bullets and the other for resetting the game. Below is how my Arduino looked like in the end:

![image](https://user-images.githubusercontent.com/24204239/120115830-a86e7b00-c196-11eb-8f38-45dc9a260844.png)

