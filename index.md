# DES222 Process Journal

## Initial Ideas
Simple initial ideas that could be expanded upon for the project:

- **Heart Shirt:** A Shirt with LEDs in a heart shape that flashes with the beating of the wearers heart.
- **Auto Lamp:** A lamp that gets brighter as the enviroment gets darker
- **Needy Robot:** A little robot that follows people and avoids obsatcles.
- **Med-Boy:** A device on the wrist/forearm that has a bunch of biometrics to monitor wearers health.
- **Shock Roulett:** More of a game, a small device that people will take turns holding that will randomly make a loud noise or small shock made more likely by how nervous the user is.

## Detailed Idea

### General Idea
Three handles connected to a main unit that holds a microbit processor. Each of the handles will have sensors to detect pluse and how sweaty the hands of the person holding the handle is and a vibration motor or some way to shock the holder. When a button on the device is pressed a "weight" is assinged to each handle based on how nervous the user by detecting their pulse and sweat of their palm. the device will then pick a handle at random, being more likely to pick a handle with a higher weight, to shock.

### Main Unit
The main unit of the prototype will be a box made out of cardboard beacuse cardboard is an easy material to work with and for the purpouses of this prototype, there are currently no other design restrictions what would require a different material. The handle would be firmly mounted in the middle on top of the box.

Alternatively the unit could have a trench for the user to rest their arm in while they grab the handle. This way the device could read the pulse from the users arm rather than their palm if the palm is too unreliable. 

The internals of the main unit would be comprised of a Micro:Bit proccessor, this is because of my familiarity with Micro:Bits but may need to be changed to a different microcontroller like an Arduino if required.

### Handles
The handles will be 3D-printed in two halfs that snap together to form an ergonomic shape for a hand. There will be varous holes in the back of the handles for the different sensors and the shock method 

### Activation / Use
I have three ideas for how the device can be activated / will be used:

1. Each handle has an individual button and the users will press the buttons individually when indicated to do so by LEDs on the main unit. When the button is pressed the device will alocate a chance of being shocked ranging from somewhere between 40% - 90% based on how nervous the device thinks the user is.

2. Theres one button on the main unit and when the button is pressed there will be a countdown and near the end of the countdown each handle's weight will be computed and the device will choose a handle to shock at random, weighted towards those that were detected to be more nervous.

3. A lose combination of the above methods, one handle connected to the main unit either by cables or being fully connected into the main unit. When the button on the handle is pressed some kind of countdown (i.e. A speaker counting down, A speaker playing a short tune, LEDs turning off) near the end of the count down a weight will be assigned based off how nervous the device thinks the user is. The device is then more likely to shock the user based on nerves in a similar range to the first idea.

Right now the prefered option is the third due to having fewer inputs to manage and a lower material cost needing to only make one handle as opposed to two.

### Method of sending Shock
There are current two ideas for how the shock will be administered to the user:

1. In the back of the handles there will be two metal strips that are covered by the user's palm making a ciruit with a small capacitor and a switch within the device, shocking the user when the circuit is completed.

2. In the handle there is a vibrating motor conncted to a small "spike" or tab in the back of the handle facing the users palm, the spike isn't sharp. When the device triggers the motor the spike will rappidly jab the users hand, causing a "shock" without inflicting any real damage.

Right now the best option of the two would be the vibrating spike mainly due to the uncertainty of how well the device could administer a shock that will suprise the user without causing them much harm.

### Additional Thoughts
A list of thoughts I had during the development of this idea that might be implemented:
- A reverse pity system where the device makes you more likley to be shocked based on how many times you haven't been.
- A way to switch between the first two modes mentioned in the Activation / Use section.
- A way for the device to detect the body heat of the user.
- Polygraph API

### Similar Examples
- **Lightning reaction reloaded**; When the button on the main unit is pressed it will go red, when it goes green players must press the button on the top of their conrolers and the last person to press their button gets shocked.

![Four handles with buttons on the top wired into a main unit with a big white button](Images/Lightning%20Reaction%20Reloaded.jpg)

- **Amazing Roulette**;  Players stick their fingers into the holes on the top of the device and one will be shocked at random.

![A black unit with two buttons on the face and six holes for players to put their fingers in](Images/Amazing%20roulette.jpg)

<!-- ## Image
![Text for accessability](Path) -->
