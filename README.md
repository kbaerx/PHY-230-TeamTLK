# PHY-230-TeamTLK
Team Homework #1

#Lizzie Apel

import random
import numpy as np 
import matplotlib.pyplot as plt
import turtle as t

def showMontePi(numDarts):
    t.up()
    t.goto(-1,0)
    t.down()
    t.goto(1,0)
    
    t.up()
    t.goto(0,1)
    t.down()
    t.goto(0,-1)
    
    circle = 0
    t.up()

    for i in range(numDarts):
        x = np.random.rand
        y = np.random.rand

        d = np.sqrt(x**2 + y**2)

        t.goto(x,y)
        
        if d <= 1:
            circle = circle + 1
            color="blue"
        else:
            color= "red"
            
        t.dot()

    pi = circle/numDarts * 4
    
    return pi
