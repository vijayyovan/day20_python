import random
from turtle import Turtle, Screen


screen = Screen()
screen.setup(width=500,height=400)
user_bet = screen.textinput(title="Make your bet",prompt="which turtle will win the race? Enter a color")
# print(user_bet)
colors = ["red", "orange", "yellow", "green", "blue", "purple"]
y_positions = [-70, -40, -10, 20, 50, 80]
all_turtles = []

# tim = Turtle(shape="turtle")

# def scoregraph(self):
for number in range(0,6):
    tim = Turtle(shape="turtle")
    tim.color(colors[number])
    tim.penup()
# tim.goto(x=230, y=100)
#     for i in range(0,3):
    tim.goto(x=-230, y=y_positions[number])
    all_turtles.append(tim)

        # tim.goto(x=230,y=)

# a = tim
# b = a.clone()
# c = a.clone()
# scoregraph(a)
# scoregraph(b)
# scoregraph(c)

if user_bet:
    is_race_on = True

while is_race_on:
    for turtle in all_turtles:
        if turtle.xcor() > 230:
            winning_color =turtle.pencolor()
            if winning_color == user_bet:
                print(f"you've won! The {winning_color} turtle is the winner")
            else:
                print(f"you've lost ! The {winning_color} turtle is the winner")
            rand_distance = random.randint(0,10)
            turtle.forward(rand_distance)



screen.exitonclick()
