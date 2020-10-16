# The Project
In my quest to find an interesting dataset to analyze I stumbled upon an old data contest presented by StockX, a popular website that allows its users to buy or sell items (most commonly—but not limited to—shoes, clothing, and accessories) at their current "market value". I mostly browse the website for high-end and rare sneakers, which is why I got excited when I found that the data that StockX provided for their contest is focused on sneaker sales.

In this project, I hope to answer the following questions:
* Are customers in certain regions more likely to spend more on sneakers?
* Is there a higher chance of making money re-selling larger shoe sizes or smaller shoe sizes?
* What is the average ROI on re-selling Yeezy shoes vs. Off-White x Nike?
* Do these sneakers sell more during a certain time of the year?
* Are Yeezy and Off-White sales increasing or decreasing?

## Results
#### Are customers in certain regions more likely to spend more on sneakers?  
StockX users in California and New York spent the most money on either Yeezy or Off-White branded shoes over the course of 2 years, about \$9.2 million and \$7.3 million, respectively. The state with the next highest sales is Oregon, with users there spending about \$3.6 million over 2 years. The remainder of the states spent less than \$3 million on Yeezy and Off-White shoes. The median amount of money spent on these shoes is only around \$280,000, which pales in comparison to the \$9.2 million users in California spent.

#### Is there a higher chance of making money re-selling larger shoe sizes or smaller shoe sizes?
Size 10 shoes were a clear winner in terms of number of pairs sold and ROI. The next top selling shoe sizes were size 11 and size 9, with size 11 shoes selling just slightly more than size 9 shoes. In terms of sales for half-sizes and full-sizes, full-sizes consistently sold more than their neighboring half-sizes.

#### What is the ROI on re-selling Yeezy shoes vs. Off-White x Nike?
In total, re-selling Off-White shoes earned about \$4 million more in ROI than Yeezys. The average ROI per pair of Off-White shoes was almost \$500, compared to the average ROI of about \$140 for Yeezys. Although selling Off-White shoes provided a much higher ROI, sellers had a much higher chance of actually selling a pair of Yeezys. Of the almost 100,000 pairs of shoes sold in the data, over 70,000 were Yeezys—in other words, a user had over a 70% chance of successfully selling a pair of Yeezys and less than 30% chance of selling an Off-White pair.

#### Do these sneakers sell more during a certain time of the year?
In the year 2018, for most of the year the number of sales remained below 7,000 sales per month, with most lingering around 3,000 to 4,000 sales per month. The data then showed a sudden increase in sales in November and December of that same year, about 10,000 and 15,000 sales, respectively. The increase in sales is most likely due to the holiday season celebrated in November and December. In terms of ROI, however, the monthly ROI was relatively high from May until December, with the exception of September. Upon further investigation, the high monthly ROIs were heavily influenced by Off-White sales, which we've previously found to have a premium price tag.

#### Are Yeezy and Off-White sales increasing or decreasing?
The data showed no clear trend that indicated increasing or decreasing sales. The data did show that sales experienced large spikes, most likely coinciding with the brands releasing a new shoe collection, followed by long periods of low sales.

## Conclusion
The results above can potentially help companies or independent sellers improve their sales performance. For instance, a shoe company that finds out that California and New York are the top two states in the sneaker market could choose to spend more of their advertising budget in those two states and less of it in, say, Wyoming. Or, independent re-sellers, who only stock up on rare shoes just a few times a year, could maximize their profits by focusing their selections on the most in-demand shoe sizes and the shoe brands that are almost guaranteed to re-sell quickly. These are just a few of the practical uses of data analysis in the sneaker market. Although this analysis is focused on Yeezy and Off-White sneaker sales, it can be expanded reflect the sales performances of a variety of brands and clothing items.

## The Data
The contest details and the [sneaker data](https://s3.amazonaws.com/stockx-sneaker-analysis/wp-content/uploads/2019/02/StockX-Data-Contest-2019-3.xlsx) is described on the [StockX contest webpage](https://stockx.com/news/the-2019-data-contest/). The website provides the following description of the data:  
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
