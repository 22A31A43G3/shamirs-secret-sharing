# shamirs-secret-sharing
Hashira Placements Assignment - Shamir Secret Sharing Reconstruction
Overview

This repository contains the solution to the Hashira Placements Assignment where the goal is to reconstruct the secret (constant term of a polynomial) from given roots (points) in JSON format using Lagrange Interpolation.

Assignment Details

Input: JSON formatted test cases with points defined by their base and value.

Output: The reconstructed secret from the minimum required number of points k.

Languages Allowed: Any except Python.

Duration: 45 minutes.

Testing: The code reads JSON input, parses it, and reconstructs the secret using Shamir Secret Sharing principles.

Implementation

The solution is implemented entirely in Java.

Utilizes BigInteger for handling large values and arbitrary bases.

Implements Lagrange interpolation to reconstruct the polynomial's secret.

Parses JSON input using standard Java libraries for easy integration with provided test cases.

How to Run

Compile the Java file:

javac ShamirSecretSharing.java


Run the program, ensuring the JSON input is correctly loaded and parsed.

Sample Input (JSON)
{
    "keys": {
        "n": 4,
        "k": 3
    },
    "1": {
        "base": "10",
        "value": "4"
    },
    "2": {
        "base": "2",
        "value": "111"
    },
    "3": {
        "base": "10",
        "value": "12"
    },
    "6": {
        "base": "4",
        "value": "213"
    }
}

Output

test case 1: 3
test case 2: -6290016743746469796

Notes

The solution has been tested manually against the sample input and verified for correctness.

The second test case can be found in the assignment link and the solution can handle it in a similar manner.

Submission

The code is pushed to the GitHub repository linked in the submission form.
