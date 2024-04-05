# Coding Challenge: Best Time to Buy and Sell Stock

This Python script tackles the problem of finding the maximum profit achievable by buying and selling a stock at different prices on consecutive days. Here's a comprehensive guide on how the script works and how to use it.

## Problem Statement

You are given an array `prices` where `prices[i]` represents the price of a given stock on the `ith` day. The goal is to maximize the profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock. If no profit can be achieved, the function should return `0`.

## Example

**Example 1:**

Input: `prices = [7,1,5,3,6,4]`  
Output: `5`  
Explanation: Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = 6 - 1 = 5.  
Note that buying on day 2 and selling on day 1 is not allowed because you must buy before you sell.

**Example 2:**

Input: `prices = [7,6,4,3,1]`  
Output: `0`  
Explanation: In this case, no transactions are done, and the max profit is `0`.

## Solution Approach

The script follows a brute force approach to find the maximum profit. It iterates through each price in the array and compares it with the prices on subsequent days. If the difference between the prices on the current day and any future day is greater than the current profit, the profit is updated.

## Function Description

The `buy_sell_stock(prices)` function takes a list of `prices` as input and returns the maximum profit that can be achieved by buying and selling the stock. If no profit is possible, it returns `0`.

## Usage

To use the script, you can call the `main()` function, which demonstrates the usage of the `buy_sell_stock()` function with the provided examples.

```python
def main():
     prices = [7,1,5,3,6,4]
     profit = buy_sell_stock(prices)
     print(profit) # Output: 5 (6 - 1)

if __name__ == "__main__":
     main()
```

Replace the `prices` list with your own stock prices array and run the script to find the maximum profit achievable.
