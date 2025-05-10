
# Simple Interest Calculator
A bash script to calculate simple interest. This project is part of a micro-finance startup's transition to Git. Open source and licensed under Apache 2.0.


#!/bin/bash

# Simple Interest Calculator

echo "Welcome to the Simple Interest Calculator"

# Read principal, rate, and time from the user
read -p "Enter the principal amount: " principal
read -p "Enter the rate of interest (in %): " rate
read -p "Enter the time (in years): " time

# Calculate simple interest
interest=$(echo "scale=2; ($principal * $rate * $time) / 100" | bc)

# Display the result
echo "The Simple Interest is: $interest"
