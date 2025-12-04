📊 Statistical Analysis Tool (Math-Skills)

A robust CLI statistical analysis tool written in Go. This program reads a dataset of numbers from a file and calculates the Average, Median, Variance, and Standard Deviation, automatically rounding the results to the nearest integer.

📑 Table of Contents

Prerequisites

Installation

Usage

Testing & Data Generation

Manual Testing

Using the Data Generator (Docker)

Algorithms Used

🛠 Prerequisites

Before running the project, ensure you have the following installed:

Go (Golang): Required to compile and run the application.

Docker (Optional): Required only if you wish to use the provided automated data generator script.

📦 Installation

Clone the repository and navigate to the project directory:

git clone <your-repo-url>
cd math-skills


🚀 Usage

To run the program, pass the filename containing your population data as an argument:

go run main.go data.txt


Example Output

After running the command above, the program will output statistics in the following format:

Average: 20
Median: 20
Variance: 67
Standard Deviation: 8


🧪 Testing & Data Generation

You can test the program in two ways: by manually creating a dataset or by using the provided Docker-based data generator.

Option 1: Manual Testing

Create a file named data.txt.

Add a list of integers (one per line).

Example data.txt:

10
20
30


Run the program:

go run main.go data.txt


Option 2: Using the Data Generator (Docker)

If you have the provided stat-bin folder and Docker installed, you can generate random datasets to stress-test the application.

1. Generate Data

Run the following script to create a data.txt file filled with random numbers:

./run.sh math-skills


⚠️ Note for Windows / Git Bash Users

If the script fails with path errors, use this manual Docker command instead:

docker run --rm -v "/$(pwd -W):/app" -w //app math-runner ./bin/math-skills


2. Run Your Solution

Once data.txt is generated, run your Go program to see the statistics:

go run main.go data.txt


🧮 Algorithms Used

The program implements the following statistical formulas, rounding all final results to the nearest integer:

Statistic

Description

Average (Mean)

Calculated by summing all values and dividing by the total count of numbers.

Median

The middle value in a sorted list. If the list has an even number of elements, it is the average of the two middle values.

Variance

The average of the squared differences from the Mean.

Standard Deviation

The square root of the Variance.

<p align="center">
<sub>Made with ❤️ in Go</sub>
</p>