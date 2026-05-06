Title: Heart-Beat Monitor (2025 UC Berkeley EE 120 Signal Processing Lab 2)

#1. Edge Detecting Filter
The *simple* moving average filter is specified in terms of a single integer parameter, $L$, which represents the length of the filter. The filter takes the average of the $L$ points before, and including, the current point of a signal, outputting that average. Formally, the filter's impulse response is:

$$h_{SMA}[n] = \frac{\delta[n] + \delta[n - 1]\ +\ ...\ +\ \delta[n - (L - 1)]}{L}$$


#2. Data Smoothing

filt_sizes = [2, 5, 10, 20, 50, 100, 500]

n = np.arange(1001)
x_exp = np.exp(n/300)
x = np.append(x_exp, np.zeros(500))
z = np.random.normal(loc=0, scale=4, size=np.shape(x))
y = z + x
plt.figure(figsize=(16, 4))
plt.plot(np.arange(len(x)), y)
plt.ylim([-25, 40])
plt.ylabel("Noised Signal")
plt.xlabel("True Signal")
plt.show()

#2.b Extracting Trends From Data
