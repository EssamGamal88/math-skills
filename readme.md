Statistical Analysis Tool (Math-Skills)
This project is a statistical analysis tool written in Go. It reads a dataset of numbers from a file and calculates the Average, Median, Variance, and Standard Deviation, rounding the results to the nearest integer.
Prerequisites
Go (Golang): Ensure Go is installed on your machine.
Docker (Optional): Required only if you wish to use the provided data generator script.
Installation
Clone the repository and navigate to the project directory:
git clone <your-repo-url>
cd math-skills


How to Run
To run the program with a data file:
go run main.go data.txt


Testing the Program
You can test the program in two ways: manually creating data or using the provided data generator.
Option 1: Manual Testing
Create a file named data.txt.
Add a list of numbers (one per line). Example:
10
20
30


Run the program:
go run main.go data.txt


Option 2: Using the Data Generator (Docker)
If you have the provided stat-bin folder and Docker installed, you can generate random datasets to stress-test the application.
Generate Data:
Run the following script to create a data.txt file filled with random numbers:
./run.sh math-skills

Note for Windows/Git Bash users: If the script fails with path errors, use this manual command:
docker run --rm -v "/$(pwd -W):/app" -w //app math-runner ./bin/math-skills


Run Your Solution:
Once data.txt is generated, run your Go program to see the statistics:
go run main.go data.txt


Example Output
Average: 20
Median: 20
Variance: 67
Standard Deviation: 8


Algorithms Used
Average: Sum of values divided by the count.
Median: The middle value in the sorted list (or average of the two middle values).
Variance: The average of the squared differences from the Mean.
Standard Deviation: The square root of the Variance.
