# PHY-230-TeamTLK
Team Homework #1

#Lizzie Apel

import random
import numpy as np 
import matplotlib.pyplot as plt

def showMontePi(numDarts):
    N =numDarts
    
    for i in range(numDarts):
        x = np.random.rand(N)
        y = np.random.rand(N)

        d = np.sqrt(x**2 + y**2)

        circle = 0
        if d <= 1:
            circle = circle + 1
            color="blue"
        else:
            color= "red"

    pi = circle/numDarts * 4
    
    return pi
