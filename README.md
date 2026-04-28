# Stock Price Analyzer | DSA Final Project

> A command-line tool for analyzing stock price data using fundamental algorithms and data structures. Built as the final project for the **Algorithms & Data Structures** course at **Superior University**.

## Project Overview
This project implements a stock price analyzer that processes 60 days of historical stock data (`stock_data.csv`). It demonstrates efficient algorithmic techniques including divide-and-conquer sorting, logarithmic search, prefix sums, and dynamic programming to solve real-world financial analysis tasks.

## Algorithms & Features
| Algorithm | Function | Time Complexity | Purpose |
|-----------|----------|-----------------|---------|
| **Merge Sort** | `merge_sort_by_price()` | `O(n log n)` | Sort stock records by price in ascending order |
| **Binary Search** | `binary_search_by_date()` | `O(log n)` | Efficiently locate stock price by date |
| **Prefix Sum** | `calculate_prefix_sum_prices()` | `O(n)` build, `O(1)` query | Precompute cumulative prices for fast range operations |
| **Kadane's Algorithm** | `kadane_max_profit()` | `O(n)` | Find optimal buy/sell dates for maximum profit |
| **Moving Average** | `calculate_moving_average()` | `O(n)` | Compute sliding-window averages using prefix sums |

## Team Members & Contributions
|    Member    | Algorithms Implemented | Role Description |
|--------------|------------------------|------------------|
| **Arman Zia** | Merge Sort | Implemented a recursive divide-and-conquer `merge_sort_by_price()` function to sort stock data without modifying the original list, ensuring `O(n log n)` performance. |
| **Mahbub Hasan** | Binary Search & Kadane's Algorithm | Developed an `O(log n)` `binary_search_by_date()` for fast date lookups and applied Kadane’s algorithm to `kadane_max_profit()`, tracking daily price changes to identify the optimal buy/sell window. |
| **Abdul Rafay** | Prefix Sum & Moving Average | Built `calculate_prefix_sum_prices()` to generate cumulative price arrays, enabling `O(1)` range queries, and leveraged it to implement an efficient sliding-window `calculate_moving_average()`. |

> 💡 *Per course requirements, all team members have reviewed, tested, and can explain every line of code in the repository.*

## 🚀 How to Run
1. Ensure `stock_analyzer.py` and `stock_data.csv` are in the same directory.
2. Run the CLI application:
   ```bash
   python stock_analyzer.py
