# 📈 Math-Skills: Statistical Analysis CLI Tool

![Go Version](https://img.shields.io/badge/Go-1.20%2B-00ADD8?style=flat&logo=go)
![Status](https://img.shields.io/badge/Status-Completed-success)

A **powerful, fast, and lightweight command-line interface (CLI) tool** for performing essential statistical analysis on datasets. Written in **Go (Golang)** for optimal performance, this tool efficiently computes key descriptive statistics.

---

## ✨ Features

The tool reads a list of integer values from a file and calculates the following metrics, with all results automatically **rounded to the nearest integer**:

* ✅ **Average** (Arithmetic Mean)
* ✅ **Median**
* ✅ **Variance**
* ✅ **Standard Deviation**

---

## 📑 Table of Contents

1.  [Prerequisites](#-prerequisites)
2.  [Installation](#-installation)
3.  [Usage](#-usage)
4.  [Example Output](#-example-output)
5.  [Algorithms Used](#-algorithms-used)
6.  [Testing](#-testing)

---

## 🛠 Prerequisites

Ensure you have the following software installed on your system:

* **Go (Golang)**: Required to build and run the application.
* **Git**: Required for cloning the repository.
* **Docker** (Optional): Only required if you plan to use the automated data generation and testing method.

---

## 📦 Installation

To get a local copy up and running, follow these simple steps:

1.  **Clone the repository:**
   git clone https://github.com/EssamGamal88/math-skills.git
cd math-skills

---

## 🚀 Usage

Execute the program by providing the path to a text file containing the dataset as a command-line argument. The file must contain **integer values, one per line**.

```bash
go run main.go data.txt
