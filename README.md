# TrajOpt - Trajectory Optimization for Matlab
TrajOpt is a matlab library that I developed while working on my PhD at Cornell, studying controller design for walking robots. Some key features of this library:

- __Easy to install -__ no dependencies outside of Matlab
- __Easy to use -__ check out the examples to see for yourself
- __Readable source code -__ easy to debug your code and figure out how the software works
- __Rapidly switch methods -__ choose from a variety of methods:
    - trapazoid rule (1st-order direct transcription)
    - hermite-simpson seperated (4th-order direct transcription)
    - multi-segment chebyshev (high-order orthogonal collocation)
    - runge-kutta (4th-order multiple shooting)

# Installation:
1. Clone or download the repository
2. Add the top level folder to your Matlab path
3. Done!

# Usage:
- Call the function `trajOpt` from inside matlab.
- `trajOpt` takes a single argument: a struct that describes your trajectory optimization problem.
- `trajOpt` returns a struct that describes the solution. It contains a full description of the problem, the transcription method that was used, and the solution (both as a vector of points and a function handle for interpolation).
- For more details, type `help trajOpt` at the command line, or check out some of the examples in the `demo/` directory.

# TrajOpt can solve problems with:
- continuous dynamics
- boundary constraints
- path constraints
- integral cost function
- boundary cost function

# Contribute:
This code is still under development, and will be from now until at least May 2016. Please contact me if you have any comments or suggestions, or create a pull request if you would like to add content.

If you are interested in contributing, here are a few possible things to do:
- Create additional demo problems
- Identify holes in the documentation
- Report bugs
- Implement new methods or features

I plan on keeping an active list of things to do under the *issues* section on GitHub.