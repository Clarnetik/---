import turtle

# создаем игровое окно
window = turtle.Screen()
window.title("Ping Pong Game")
window.bgcolor("black")
window.setup(width=600, height=400)

# создаем левую ракетку
left_pad = turtle.Turtle()
left_pad.speed(0)
left_pad.shape("square")
left_pad.color("white")
left_pad.shapesize(stretch_wid=5, stretch_len=1)
left_pad.penup()
left_pad.goto(-250, 0)

# создаем правую ракетку
right_pad = turtle.Turtle()
right_pad.speed(0)
right_pad.shape("square")
right_pad.color("white")
right_pad.shapesize(stretch_wid=5, stretch_len=1)
right_pad.penup()
right_pad.goto(250, 0)

# создаем мяч
ball = turtle.Turtle()
ball.speed(40)
ball.shape("circle")
ball.color("white")
ball.penup()
ball.goto(0, 0)
ball.dx = 2
ball.dy = -2

# создаем счетчик
score_left = 0
score_right = 0
score = turtle.Turtle()
score.speed(0)
score.color("white")
score.penup()
score.hideturtle()
score.goto(0, 180)
score.write
