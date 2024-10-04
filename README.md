# Challenge 4 - Bullet Time


For this challenge, we followed and executed instructions on how to shoot game objects from assets!

---

## Player Movement

### Script
For our player movement in script, we first added a new script where we would write the code. Clicking on the character, to the left where the 'Inspector' window appears, scroll all the way down and click Add Component > New Script, we named it 'Movement'. Afterwards, we opened the new script and began coding the keys/arrows we wanted to use to move our character.

First create two public float variables, one for speed and one for the speed rotation our character will have.

<img width="286" alt="Screenshot 2024-10-04 at 3 35 26 PM" src="https://github.com/user-attachments/assets/c07e140a-8ae8-4721-bb82-81b9d2ddb706">

Then below the update, we used the general keys in PC games for movement:

W or up arrow - move forward

S or down arrow - move back

A or left arrow - move left

D or right arrow - move right

The varible mouseX is to use the mouse as our player rotations. Wherever you point to, its where you move to.

#### Complete Code:

<img width="971" alt="Screenshot 2024-10-04 at 3 37 23 PM" src="https://github.com/user-attachments/assets/549363f9-27c0-4a5a-ac84-6d1744ea66ef">

_Note:_ make sure you update your variables in unity and give them a value, as well to have your script checked.

<img width="293" alt="Screenshot 2024-10-04 at 3 49 52 PM" src="https://github.com/user-attachments/assets/8a1a9763-a93d-436e-a91c-f5ecb0ec6491">


### Final Result: 


### Visual Graph
For our player movement on visual graph, we first added a new script machine where we would write the code. Clicking on the character, to the left where the 'Inspector' window appears, scroll all the way down and click Add Component > Visual Scripting > Script Machine. Afterwards we simply translated our C# instructions into graph instructions. Make sure you check out the done script and check in there

We created our speed and speed rotation variables and gave them some values:

<img width="335" alt="Screenshot 2024-10-04 at 3 54 50 PM" src="https://github.com/user-attachments/assets/59b6967c-609c-4a71-80c3-b2400e8604f8">


Next we searched added these nodes for our player rotation:

<img width="720" alt="Screenshot 2024-10-04 at 3 58 18 PM" src="https://github.com/user-attachments/assets/0db56a78-e42d-4255-b776-d0b47fec3ef1">


For our movement with the keys, we added these nodes per group: forward, backward, left and right.

<img width="928" alt="Screenshot 2024-10-04 at 3 58 28 PM" src="https://github.com/user-attachments/assets/82ee85c2-0dae-4aec-b06f-c85b4a170368">

_Note:_ on your left and back groups, make sure you multiply your speed by -1 so it moves where you want it to since the values will hit negative.


#### Complete Graph:

<img width="384" alt="Screenshot 2024-10-04 at 3 54 21 PM" src="https://github.com/user-attachments/assets/d51a6e9a-2be1-419c-978a-4a1ec0e97c62">

### Final Result: 

[gif de graph]

## Bullets

### Bullet Prefab: 
For the bullet, we first created a sphere (GameObject > 3D Object > Sphere) and scaled it down to a small size.

<img width="300" alt="Screenshot 2024-10-04 134242" src="https://github.com/user-attachments/assets/acaf376c-14b3-4ffa-83da-45480abd67a4">

Then we created a new material by right clicking > Create > Material in the assets area or by clicking the ‘+’ symbol > Material.

<img width="385" alt="Screenshot 2024-10-04 133959" src="https://github.com/user-attachments/assets/0f89feb3-595c-4d58-b969-8d4ed8ec6944">

In the inspector tab of the material, within Surface Inputs, we changed the Base Map to our choice of color and added an emission for a glowing effect. 

<img width="300" alt="Screenshot 2024-10-04 134147" src="https://github.com/user-attachments/assets/f2be6b3f-7f4f-41d3-a2ce-977a74201218">

Then we dragged the material onto the sphere previously created. 

<img width="300" alt="Screenshot 2024-10-04 134252" src="https://github.com/user-attachments/assets/31d19f82-db86-46df-97ff-50adc5713589">

With the bullet’s look completed, we turned it into a prefab by dragging the object from the Hierarchy tab onto a prefab folder.

## Script:
Within the prefab of the bullet, in the inspector tab, we created a script (Add Component > New script) which we named “forwardMovement”. 
For this script, we added the public variable 'speed' and the following code for the purpose of providing movement for when the bullets are shot out.

<img width="500" alt="Screenshot 2024-10-04 160802" src="https://github.com/user-attachments/assets/0e0f3c9e-8f1a-4f60-95b8-3f25db26401b">

Lastly, in Unity, be sure to change the value of the speed.

<img width="350" alt="Screenshot 2024-10-04 161136" src="https://github.com/user-attachments/assets/eb0a6659-a6c3-46ef-9e1e-607e77ed9873">

## Shooting Bullets
For the character to shoot the bullets, we first had to create an empty object (GameObject > empty) which we referred to as ShootPoint, positioned it where we would want the bullets to come out of and then moved the object onto the hierarchy of the asset.

<img width="600" alt="Screenshot 2024-10-04 140608" src="https://github.com/user-attachments/assets/f022df58-7cca-44ba-ac3b-b7dc88f62510">

Then, we edited the Movement script from the asset to add two public GameObject variables called ‘prefab’ and ‘shootPoint’.

<img width="286" alt="Screenshot 2024-10-04 170922" src="https://github.com/user-attachments/assets/d7e90ed0-e2ed-4cc6-8f48-e34ed01035c8">

Continuing, we added the following code that creates an instance/copy of the bullet prefab and positions it where the shooting point object is located once the left mouse button is pressed.

<img width="450" alt="Screenshot 2024-10-04 170848" src="https://github.com/user-attachments/assets/61122b65-b0e5-4f76-8469-c706b8ada777">

The newly modified script should look like this:

Variables:

<img width="300" alt="Screenshot 2024-10-04 170801" src="https://github.com/user-attachments/assets/b543119a-6959-481f-b6ea-a9429643c1ad">

Code:

<img width="900" alt="Screenshot 2024-10-04 170832" src="https://github.com/user-attachments/assets/bc9f249f-2b3b-409e-b3ed-e7971433684e">

Lastly, back in Unity, be sure to drag the bullet prefab and the shootPoint object to their corresponding variables.

<img width="350" alt="Screenshot 2024-10-04 161206" src="https://github.com/user-attachments/assets/09a3b2d7-8a1d-45f6-ba20-fd0acf25a3e8">

_Note:_ make sure the C# script is checked and the graph un-checked before running the program.

### Final Result

![shooting-ezgif com-crop](https://github.com/user-attachments/assets/411a955e-e1a2-45f8-b191-5e7faf31a3f9)

## Experienced Gained:



