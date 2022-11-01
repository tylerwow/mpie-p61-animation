# Practical 6.1: Animation in Maya

In the first lecture this week we learned about some key principles of animation in 3D environments, and how we can work with them in Maya. In this practical, you’re going to put that learning into action and do some of the things that were shown in the lecture. 

By the end of this practical, you’ll be able to bring objects and even characters to life – making scenes that are dynamic and realistic. In particular you’ll be able to:

- Create an animated piece of scenery
- Rig your first character
- Combine all of these skills to create an animated character!

In this practical, you’ll be using Maya. This is already installed for you on our lab machines. However, if you’d like to continue to work with it on your personal machine, you can get a free educational license here:

https://www.autodesk.com/education/edu-software/overview?sorting=featured&filters=individual

You can find some assets you'll be using during this practical in this template Git repository. The best way to access these is to create a new respository from the template in your account and clone it onto the machine you're working on.

## Task 1: Unlocking the Airlock

In this task we’re going to create our first simple animation: the lock mechanism opening on a sliding airlock door. To get started, open the airlock.fbx model in Maya. You can do this by dragging it into a new scene. Once you’ve opened the model press ‘6’ on your keyboard to see the textured display.

Take a look at the model; you’ll see it’s an airlock that could be included in a space station scene. If you open the outliner (Windows > Outliner) you’ll see there are three main elements of the model:

-	The surrounding walls (airlock_chamber)
-	The doors (door_left, door_right)
-	Some lock bolts that can move independently (bolt_left, bolt_right)

*Tip: in case you’ve not seen the Maya Outliner before, it’s just like the hierarchy view in Unity. You can use it to see all of the elements in your scene and how they relate to each other in terms of parent and child relationships – its really useful!*

In the first task, you should use what you learned in the lecture to animate the lock bolts so that they move outwards over a period of 10 frames. The finished result should look something like this:

https://www.youtube.com/watch?v=oXExEj6YUYE

Some quick tips to help you achieve this task:

-	Consider animating just one of the bolts first – keep it simple
-	You can use ‘S’ to quickly set a key on an object
-	Set the position on the timeline when you want the key to happen before you manipulate the object to the position you want to be in
-	If the timeline is too long, you can change its length by clicking on the little running person in the bottom right of the UI
