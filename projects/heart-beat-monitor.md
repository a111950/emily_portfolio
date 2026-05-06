Title: Heart-Beat Monitor (2025 UC Berkeley EE 120 Signal Processing Lab 2)

#1. Edge Detecting Filter
The *simple* moving average filter is specified in terms of a single integer parameter, $L$, which represents the length of the filter. The filter takes the average of the $L$ points before, and including, the current point of a signal, outputting that average. Formally, the filter's impulse response is:

$$h_{SMA}[n] = \frac{\delta[n] + \delta[n - 1]\ +\ ...\ +\ \delta[n - (L - 1)]}{L}$$

#2. Data Smoothing

#2.b Extracting Trends From Data
