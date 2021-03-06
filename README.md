# Dynamic_Pricing_Airline_Challenge
This is solution to the Airline Price Optimization Micro-Challenge
The Problem
You recently started Aviato.com, a startup that helps airlines set ticket prices.

Aviato's success will depend on a function called pricing_function. This notebook already includes a very simple version of pricing_function. You will modify pricing_function to maximize the total revenue collected for all flights in our simulated environment.

For each flight, pricing_function will be run once per (simulated) day to set that day's ticket price. The seats you don't sell today will be available to sell tomorrow, unless the flight leaves that day.

Your pricing_function is run for one flight at a time, and it takes following inputs:

Number of days until the flight
Number of seats they have left to sell
A variable called demand_level that determines how many tickets you can sell at any given price.
The quantity you sell at any price is:

quantity_sold = demand_level - price

Ticket quantities are capped at the number of seats available.

Your function will output the ticket price.

You learn the demand_level for each day at the time you need to make predictions for that day. For all days in the future, you only know demand_level will be drawn from the uniform distribution between 100 and 200. So, for any day in the future, it is equally likely to be each value between 100 and 200.
