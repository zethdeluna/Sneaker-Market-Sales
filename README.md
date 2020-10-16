# The Project
In my quest to find an interesting dataset to analyze I stumbled upon an old data contest presented by StockX, a popular website that allows its users to buy or sell items (most commonly—but not limited to—shoes, clothing, and accessories) at their current "market value". I mostly browse the website for high-end and rare sneakers, which is why I got excited when I found that the data that StockX provided for their contest is focused on sneaker sales.

In this project, I hope to answer the following questions:
* Are customers in certain regions more likely to spend more on sneakers?
* Is there a higher chance of making money re-selling larger shoe sizes or smaller shoe sizes?
* What is the average ROI on re-selling Yeezy shoes vs. Off-White x Nike?
* Do these sneakers sell more during a certain time of the year?
* Are Yeezy and Off-White sales increasing or decreasing?

## The Data
The [contest details](https://stockx.com/news/the-2019-data-contest/) and the [sneaker data](https://s3.amazonaws.com/stockx-sneaker-analysis/wp-content/uploads/2019/02/StockX-Data-Contest-2019-3.xlsx) is described on the StockX contest webpage. The website provides the following description of the data:  
"The data we’re giving you consists of a random sample of all Off-White x Nike and Yeezy 350 sales from between 9/1/2017 (the month that Off-White first debuted “The Ten” collection) and the present. There are 99,956 total sales in the data set; 27,794 Off-White sales, and 72,162 Yeezy sales. The sample consists of U.S. sales only. To create this sample, we took a random, fixed percentage of StockX sales (X%) for each colorway, on each day, since September 2017. So, for each day the Off-White Jordan 1 was on the market, we randomly selected X% of its sale from each day. (It’s not important to know what X is; all that matters is that it’s a random sample, and that the same fixed X% of sales was selected from every day, for every sneaker)."

Term Definitions:
* `Order Date`: date that a user placed an order on the shoes
* `Brand`: brand name, either Yeezy or Off-White
* `Sneaker Name`: name of the sneaker
* `Sale Price`: price (\$USD) that the shoes were sold at
* `Retail Price`: original price (\$USD) of the shoes when released by the company
* `Release Date`: date that the company released the shoes for the public to purchase
* `Shoe Size`: US size of the shoes
* `Buyer Region`: state of origin of the user that purchased the shoes
