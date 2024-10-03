# color-import turtle
import random

# Define a list of colors
colors = ["red", "blue", "green", "yellow", "purple", "orange", "pink", "cyan", "magenta"]

def display_random_color():
    # Set up the turtle screen
    screen = turtle.Screen()
    screen.setup(width=400, height=400)  # Set window size
    screen.title("Random Color Display")

    # Pick a random color from the list
    random_color = random.choice(colors)
    
    # Create a turtle to fill the screen
    turtle.bgcolor(random_color)  # Set background to the random color

    print(f"The random color is: {random_color}")  # Output the chosen color
    
    # Exit on click
    screen.exitonclick()

# Run the color display function
display_random_color()
