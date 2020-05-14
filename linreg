import numpy as np
import random
import scipy
from scipy import stats

a = [] #your first list here
b = [] #your second list here
#the following is used to generate random numbers to test the code
#for i in range(0, 10):
#    num = random.randint(0, 100)
#    a.append(num)
#for i in range(0, 10):
#    nums = random.randint(0, 1000)
#    b.append(nums)
#print(a)
#print(b)

def linearize(a, b):
    newlist_a = np.array(a)
    newlist_b = np.array(b)
    return scipy.stats.linregress(newlist_a, newlist_b)
slope = linearize(a, b)[0]
intercept = linearize(a, b)[1]
rvalue = linearize(a, b)[2]
p_value = linearize(a,b)[3]
standard_error = linearize(a, b)[4]

print("y = {}x + {}".format(slope, intercept))
print("r-value of {}, p-value of {}, and standard error of {}".format(rvalue, p_value, standard_error))
