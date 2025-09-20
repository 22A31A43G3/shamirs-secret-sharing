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
sample input 2:

{
"keys": {
    "n": 10,
    "k": 7
  },
  "1": {
    "base": "6",
    "value": "13444211440455345511"
  },
  "2": {
    "base": "15",
    "value": "aed7015a346d635"
  },
  "3": {
    "base": "15",
    "value": "6aeeb69631c227c"
  },
  "4": {
    "base": "16",
    "value": "e1b5e05623d881f"
  },
  "5": {
    "base": "8",
    "value": "316034514573652620673"
  },
  "6": {
    "base": "3",
    "value": "2122212201122002221120200210011020220200"
  },
  "7": {
    "base": "3",
    "value": "20120221122211000100210021102001201112121"
  },
  "8": {
    "base": "6",
    "value": "20220554335330240002224253"
  },
  "9": {
    "base": "12",
    "value": "45153788322a1255483"
  },
  "10": {
    "base": "7",
    "value": "1101613130313526312514143"
  }
}

output:

test case 2: -6290016743746469796

Notes

The solution has been tested manually against the sample input and verified for correctness.

The second test case can be found in the assignment link and the solution can handle it in a similar manner.

Submission

The code is pushed to the GitHub repository linked in the submission form.
