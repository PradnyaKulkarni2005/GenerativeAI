import numpy as np
import matplotlib.pyplot as plt
# generative linear data without noise
# parameters
# slope
m=2
b=5 #intercept

# generate x values Start = 0 , Stop = 10 ,num = 100
x=np.linspace(0,10,100)
# generating corresponding y values
y = m * x + b
# plot
plt.figure(figsize=(8, 4))
plt.plot(x,y,label = 'True Line')
plt.xlabel('x')
plt.ylabel('y')
plt.title('Linear function without noise')
plt.legend()
plt.grid(True)
plt.show()

# add gaussian noise
# np.random.normal(0, 2, ...): draws samples from a normal (Gaussian) distribution:
# Mean (μ) = 0 → the noise is centered around zero
# Standard deviation (σ) = 2 → controls how spread out the noise is
# size=y.shape: ensures we generate as many noise values as there are y-values (100 in this case)
# So now, you have an array noise of shape (100,)
noise = np.random.normal(0,2,size=y.shape) # mean = 0 , std =2

# This adds the noise to each value of the original y.
y_noisy = y+ noise

# plotting noisy data
plt.figure(figsize=(8, 4))

# scatter(...): plots individual points (x, y_noisy)
# Red dots represent the noisy observations.
# They're scattered around the true line because of the added noise.
# alpha=0.6: makes the points a bit transparent

plt.scatter(x,y_noisy,color='red',label='Noisy Data' , alpha = 0.6)
plt.plot(x,y,label = 'True Line',color='blue')
plt.xlabel('x')
plt.ylabel('y')
plt.title('Linear function with Gaussian noise')
plt.legend()
plt.grid(True)
plt.show()

