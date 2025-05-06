# Python-Group-Assignment2.0-

# Virtual Pet Simulator

A Python implementation of a virtual pet game using Object-Oriented Programming (OOP) concepts. The game allows you to create and interact with a digital pet that can eat, sleep, play, and learn tricks.

## Features

The [`Pet`](week1.py) class implements the following features:

- Pet attributes tracking:
  - Hunger level (0-10)
  - Energy level (0-10)  
  - Happiness level (0-10)
  - List of learned tricks

- Pet actions:
  - Eating (reduces hunger, increases happiness)
  - Sleeping (restores energy)
  - Playing (requires energy, increases happiness, increases hunger)
  - Training (learns new tricks)

## Usage

```python
# Create a new pet
my_pet = Pet("Roxy")

# Check pet's status
my_pet.get_status()

# Basic interactions
my_pet.eat()      # Feed your pet
my_pet.sleep()    # Let your pet rest
my_pet.play()     # Play with your pet

# Training
my_pet.train("sit")        # Teach a new trick
my_pet.train("roll over")  # Teach another trick
my_pet.show_tricks()       # Display all learned tricks
```

## Game Mechanics

- Hunger decreases by 3 when eating (minimum 0)
- Energy increases by 5 when sleeping (maximum 10)
- Playing requires at least 2 energy points
- Playing decreases energy by 2 and increases happiness by 2
- Training new tricks costs 1 energy point and increases happiness by 1

## Example Output

```
Roxy's Status:
Hunger: 5/10
Energy: 5/10
Happiness: 5/10

Roxy is eating. Yum!
Roxy is playing and having fun!
Roxy learned to sit!
Roxy learned to roll over!

Roxy's tricks:
- sit
- roll over

Roxy is sleeping. Zzz...
```
