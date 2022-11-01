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

## Task 2: Opening the Pod Bay Doors
Now the door is unlocked, we need to open it up so players can pass through. In this task, use the same approaches you applied to animate the bolts to animate the doors. The doors should open between frames 10 and 90, and the bolts should move with the doors in the open position. The finished result should look something like this:

https://www.youtube.com/watch?v=zDTr4n1BlmQ

Getting the bolts to move with the doors is the tricky aspect of this task. However, you can achieve this quite easily if you select both the bolt and the door (either in the scene or the outliner) and manipulate and key them together.

You can apply the principles you’ve learned in the last two tasks to animate a whole range of objects in your scenes. Remember, you can key pretty much anything in Maya. Therefore, don’t just limit your animations to translational movement.

# Task 3: Rigging Your First Character
Animating the 3D models that make up the scenery of your 3D environments is crucial for a realistic effect in many cases. However, when we think of 3D animation, its common to want to animate the characters in our scenes too. In the remainder of this practical we’re going to learn how to rig and animate a human character.

To get started, open up the zombie.fbx file from the practical resources folder in a new Maya scene. You should see a 3D model of a Zombie. If you don’t see the textures on the model, press ‘6’. In this task, we’re going to create a skeletal rig that’ll let us animate the complex mesh of this character using some simpler geometry. This rig will also have the kind of human inverse kinematics model we discussed in the lecture applied to it – so some of the hard work of making realistic human movements will be done for us!

Rigging a human character in Maya is actually quite simple – if you just want a basic human that behaves in a fairly standard way. All you need to do is follow these steps using Maya’s “Quick Rig” tool:

1.	Select the mesh of the 3D character that you would like to rig (in this case the Zombie)
2.	Choose “Skeleton >> Quick Rig” from the menu
3.	Make sure that “one click” is selected at the top of the dialog box that appears
4.	Press the “auto-rig” button and wait until the rigging process completes

Tip: To find the Skeleton menu you’ll need to choose “Rigging” from the drop down box at the top left of the Maya UI

Once you’ve done this, you should now see that your character has a yellow skeleton in alignment with its main body parts. If you can’t see the skeleton, make sure that “X-Ray Joints” is selected in the “Shading” menu at the top of the scene view.

You should also see some little red circles and squares around some of the main parts of the character’s body (e.g. hands, hips, head, feet). These are called controllers, and we can manipulate the character by moving and rotating these.

Have a go at manipulating these controllers to put the character in some different poses (e.g. bending over, crouching, waving). When doing this you should notice two things that make animating characters a lot easier than it could be:

•	The inverse kinematics model moves the skeleton in a way that respects the mechanical constraints of the human body (in most cases!)
•	The controllers are hierarchical, meaning that if you, for example, move the hips, the shoulders will move too.

At this point, save a back up of your rigged character. It’ll make it easier to create animations from scratch over the next two tasks.

