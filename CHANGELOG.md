# Change Log

## 2025-01-04

During this week, Chase developed some early test code to simulate the location and reliability
of the delivery agents. Spencer spent some time developing code that can generate orders on
demand. When these two files get combined, they can generate data that looks something like the
data provided to us by the client.

We plan to use this data to experiment with various choice algorithms on how to choose between
different subcontractors.

In terms of next steps, we need to develop an algorithm for choosing these subcontractors and run
it in simulation. Our main blocker is we don't know what algorithms will work well so we need to
do some research prior to writing more code

**New files**

* `src/simulation/delivery_agents.py`
* `src/simulation/orders.py`
* `scripts/simulate.py`

