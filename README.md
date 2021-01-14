# Answering Business Questions using SQL

This project will use SQL to answer business questions based off the [Chinook database](https://github.com/lerocha/chinook-database). The Chinook database represents a digital media store with tables for artists, albums, media tracks, invoices, and customers.

## Methodology
Using SQL (for analysis) and Python (for plotting) the following questions will be answered:

1. Which albums should we purchase for the US store, based off the current best selling genres?
2. How are sales staff performing?
3. How are sales varying by country?
4. Are customers purchasing whole albums or just individual tracks?
5. Is the range of tracks in the store reflective of their sales popularity?
6. How many tracks have been purchased vs not purchased?

## The main findings are:

1. I would recommend purchasing Red Tone (Punk), Slim Jim Bites (Blues), and Meteor and the Girls (Pop). However to increase sales quickly I would suggest adding some more Rock albums as these make up 53% of total sales.
2. The total sales per employee is correlated to their hire date, with sales increasing the longer an employee has been at the firm.
3. Sales are highest in the US where we have the most customers. It would also be worth looking into increasing the number of customers from the Czech Republic, Portugal, and India because these countries have the highest sales value per customer.
4. Whole album purchases make up almost a fifth (18.57%) of invoices.
5. There is a notable mismatch between the amount of stock held for some genres and their sales popularity. For example: Rock tracks make up over 55% of sales and yet represent only 37% of stock. It may be that increasing the variety of rock tracks will generate more sales given the genre's popularity with customers. Whilst Latin tracks comprise 16% of stock but only 3% of sales. It seems unprofitable to add any more Latin genre tracks to the store unless customer tastes are expected to shift favourably towards them in future.
6. Over 45% of tracks in the store have never been purchased. This suggests that management could save money by not stocking certain tracks, and should focus on artists/albums that are more popular with existing customers. When broken down by genre it becomes clear that tracks from certain genres should not be stocked at all.

## Selected output

1. Which albums should we purchase for the US store, based off the current best selling genres?

![us sales by genre](/output/us_sales_by_genre.png)

2. How are sales staff performing?

![sales by staff](/output/sales_by_staff.png)

5. Is the range of tracks in the store reflective of their sales popularity?

![genres popularity](/output/genres_popularity.png)

6. How many tracks have been purchased vs not purchased?

![tracks not purchased by genre](/output/tracks_not_purchased_by_genre.png)

## Installation

First clone the repository in a local folder
```
git clone https://github.com/vivek-kotecha/sql-chinook.git
```
then run the scripts from the terminal with

```
python {filename}.py
```
or
```
python3 {filename}.py
```

## Dependencies

A comprehensive list of current dependencies include the following libraries
```
Sqlite3 (database management)
Pandas (data manipulation)
Numpy (scientific computing)
Matplotlib (plotting)
Seaborn (plotting)
```
