# PHY-230-TeamTLK
Team Homework #1

import random
import numpy as np 
import matplotlib.pyplot as plt

def showMontepi(numDarts):
    n=numDarts
    circle=0
    np.arange(0,1,10)
    
    for i in range(n):
        x = np.random.random()
        y = np.random.random() 
        plt.plot(x,y,'go')
        d = math.sqrt(x**2 + y**2)
        
        if d <= 1:
            circle = circle + 1
            color= 'b'
        else:
            color= 'r'
            
        
        pi = circle/n * 4

    plt.show()
    return pi
