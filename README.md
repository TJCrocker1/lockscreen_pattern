# lockscreen_pattern
Count the number of possible lockscreen patterns given pattern length and starting position.

The standard lockscreen pattern on mobile phones is made by connecting a sequence of points on a three by three grid. Each point can only be used once. A connection may be formed between the latest point in the sequence and any other unused point so long as the line connecting them does not intersect a third unused point. Where an intersected point has already been used it can be 'jumped' to allow connection between two points on it’s opposite sides.

The function count_patterns_from() takes two arguments defining the pattern length (i.e. the number of connections) and starting position (i.e. the position of the first point). The script implements a depth-first search by recursively adding unused points to the sequence and checking their validity. Each time a valid sequence of sufficient length is created a global counter is updated. When all combinations have been tested the value of the counter is returned as an integer.

Further challenge details can be found at: https://www.codewars.com/kata/585894545a8a07255e0002f1
