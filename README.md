# SUVAT Dynamics Calculator - Using the html
A browser-based physics calculator that solves constant-acceleration motion problems using the five SUVAT variables:

- **S** – Displacement  
- **U** – Initial Velocity  
- **V** – Final Velocity  
- **A** – Acceleration  
- **T** – Time  

Enter **any 3 values**, click **Calculate**, and the remaining variables are solved automatically.

## Features

- Solves all mathematically valid 3-variable combinations  
- Uses all 5 SUVAT equations  
- Iterative constraint-based solver  
- Supports unit conversion  
- Handles invalid / impossible inputs  
- Clean, minimal UI  

## Physics Assumption

This solver assumes:

> **Constant acceleration motion in one dimension**

The equations used internally:

1. `v = u + at`
2. `s = ut + ½at²`
3. `v² = u² + 2as`
4. `s = (u + v)/2 × t`

All calculations are performed in **SI units internally**, regardless of input units.

## Supported Units

| Variable | Units |
|----------|--------|
| Distance (S) | m, cm, km |
| Velocity (U, V) | m/s, km/h |
| Acceleration (A) | m/s², cm/s² |
| Time (T) | seconds |

## How It Works

Instead of using hardcoded condition chains, the solver:

1. Converts inputs into SI units.
2. Iteratively applies all SUVAT equations.
3. Propagates new values when solvable.
4. Stops when no further variables can be computed.
5. Converts results back to selected units.

This makes it flexible and mathematically complete for constant acceleration motion.

---

# SUVAT Dynamics Calculator - Using main.c

This program calculates the unknown data from the 4 basic formulas of dynamics (SUVAT) if you know the values of any 3 of these, you can find the other 2 easily. The program is designed to take inputs in the MKS (Meter, Kilogram, Second) units and provide output in the same.

## Information

The program defines unknown data using the 4 basic formulas of dynamics, commonly referred to as 'SUVAT':
- **s**: Distance traveled
- **u**: Initial velocity
- **v**: Final velocity
- **a**: Acceleration
- **t**: Time of travel

## Instructions

1. **Input all data in MKS units (Meter, Kilogram, Second).**
2. **The program will provide output in MKS units.**

## Usage

### Find Distance Traveled (s)

1. Press `s` to find the distance traveled.
2. Enter the data you have:
   - `1`: Starting velocity, acceleration, and time of travel
   - `2`: Starting velocity, ending velocity, and acceleration
   - `3`: Starting velocity, ending velocity, and time

### Find Initial Velocity (u)

1. Press `u` to find the starting velocity.
2. Enter the data you have:
   - `1`: Distance, acceleration, and time of travel
   - `2`: Distance, ending velocity, and time of travel
   - `3`: Distance, acceleration, and ending velocity
   - `4`: Ending velocity, acceleration, and time of travel

### Find Final Velocity (v)

1. Press `v` to find the ending velocity.
2. Enter the data you have:
   - `1`: Distance, starting velocity, and time of travel
   - `2`: Distance, starting velocity, and acceleration
   - `3`: Starting velocity, acceleration, and time of travel

### Find Acceleration (a)

1. Press `a` to find the acceleration.
2. Enter the data you have:
   - `1`: Distance, starting velocity, and time of travel
   - `2`: Distance, starting velocity, and ending velocity
   - `3`: Starting velocity, ending velocity, and time of travel

### Find Time of Travel (t)

1. Press `t` to find the time of travel.
2. Enter the data you have:
   - `1`: Distance, starting velocity, and acceleration
   - `2`: Distance, starting velocity, and ending velocity
   - `3`: Starting velocity, ending velocity, and acceleration

## Example

To find the distance traveled given the starting velocity, acceleration, and time of travel:
1. Press `s`.
2. Press `1` to select starting velocity, acceleration, and time of travel.
3. Enter the starting velocity, acceleration, and time of travel when prompted.

## Note

Please enter valid inputs as prompted by the program. Any invalid entries will result in an "Invalid Entry" message.

## Acknowledgements

This program has entirely been written by K.M. Najib Hayder in 2021.
