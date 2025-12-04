📊 Math-Skills: Statistical Analysis CLI Tool

A powerful and fast command-line statistical tool written in Go, designed to analyze datasets and compute:

✅ Average
✅ Median
✅ Variance
✅ Standard Deviation

All results are automatically rounded to the nearest integer.

<p align="center"> <img src="https://img.shields.io/badge/Language-Go-blue?style=for-the-badge" />  <img src="https://img.shields.io/badge/Docker-Supported-2496ED?style=for-the-badge&logo=docker&logoColor=white" /> </p>
📑 Table of Contents

Prerequisites

Installation

Usage

Example Output

Testing & Data Generation

Manual Testing

Docker-Based Testing

Algorithms Used

🛠 Prerequisites

Make sure you have the following installed:

Go (Golang) — to compile & run the app

Docker (Optional) — only required for automated dataset generation

📦 Installation
git clone <your-repo-url>
cd math-skills

🚀 Usage

Run the program by passing a file containing integer values (one per line):

go run main.go data.txt

🧾 Example Output
Average: 20
Median: 20
Variance: 67
Standard Deviation: 8

🧪 Testing & Data Generation

You can test the tool in two different ways.

🔹 Option 1: Manual Testing

Create a file named data.txt

Add numbers, one per line:

10
20
30


Run the program:

go run main.go data.txt

🔹 Option 2: Docker Data Generator

If you have the provided stat-bin folder, you can auto-generate datasets.

1. Generate Random Data
./run.sh math-skills

⚠️ Windows (Git Bash) Users

If the script gives path issues, run:

docker run --rm -v "/$(pwd -W):/app" -w //app math-runner ./bin/math-skills

2. Run Your Solution
go run main.go data.txt

🧮 Algorithms Used
Statistic	Description
Average (Mean)	Sum of all values ÷ count
Median	Middle value after sorting (or mean of two middle values)
Variance	Average of squared differences from the mean
Standard Deviation	Square root of the variance

All results are rounded to the nearest integer.

<p align="center"> <sub>Made with ❤️ using Go</sub> </p>