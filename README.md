# Challenge 4 - Bullet Time


For this challenge, ni se que poner aqui 

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
[gif de script]

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

## Bullet Prefab

## Shoot Bullet

## Experienced Gained:



