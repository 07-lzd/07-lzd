import turtle
import random
import time

#发射烟花

def firework(t):
    t.hideturtle()
    t.pensize(2)
    t.speed(10)
    for i in range(18):
        t.forward(100)
        t.backward(100)
        t.right(20)
        t.showturtle()

        
#绽放烟花
        
def explode(t):
    t.pensize(2)
    for i in range(30):
        t.color(random.random(),random.random),
        random.random()
        t.forward(15)
        t.backward(15)
        t.right(12)

        
#设置画布
        
screen=turtle.Screen()
screen.bgcolor("black")

#创建多个烟花

for _ in range(num_fireworks):
    t=turtle.Turtle()
    x=random.randint(-200,200)
    y=random.randint(-200,200)
    t.penup()
    t.goto(x,y)
    t.pendown()
turtles.append(t)

#循环展示烟花效果
               
for t in turtles:
               firework(t)
               time.sleep(1)
               explode(t)
               time.sleep(1)


