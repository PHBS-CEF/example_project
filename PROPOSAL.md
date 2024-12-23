# Consulting project proposal

**Group members**: Chase Coleman, Spencer Lyon, Thomas Sargent


## Project description

We are interacting with a company that specializes in delivery. The company has had issues with
customer retention due to an inconsistent ability of subcontractors to make deliveries within the
expected window.

The issue here is two-fold:

1. The company chooses a subcontractor and makes an estimate for how long the subcontractor will
  take to make the delivery. They believe their estimates are reasonable but it is possible that
  they are being over-optimistic -- A reliable estimate, even if slightly longer than current
  estimates, may be better in terms of customer expectations.
2. The subcontractors may not make a delivery within the specified window for reasons that are
  outside of the company's control -- For example, they may stop and eat lunch even though they
  have been assigned a particular delivery route which can delay the customer's delivery. The
  company would like to route as many deliveries as possible to the most reliable subcontractors
  to create incentives for being reliable and delivering in a timely manner. Obviously, being able
  to estimate what is a timely manner is important for this -- If you only allocate 10 minutes for
  delivery that takes no less than 30 minutes then you may be penalizing reliable subcontractors.

The company currently has live data tracking capabilities. This allows them to see things like
(1) an order as it comes in (along with relevant data like where the order is), (2) where the
subcontractors are as an order comes in, (3) whether an order has been fulfilled.

The company would like us to help them resolve one or both of the issues described above.

We believe that task 2 will have a larger immediate impact on the company's success so we will
proceed to develop solutions for that task.


## Data description

The data that the company has provided is proprietary. We have instead generated a ficticious
dataset with many of the same properties as the original data. To keep things simple, we will
restrict to 50 possible subcontractors and 5 approximate locations (think about these as
"neighborhoods").

The data has one row per order that occurs. Each row contains:

* Time ordered
* Neighborhood where delivery should occur
* Estimated time to delivery from the app
* Location of each of the 50 subcontractors -- They are given a -1 if they are busy or offline


## Task breakdown

The end goal of our project is to have an algorithm that is able to choose a subcontractor in real
time as delivery orders come in.

The big steps that we believe need to be taken are:

1. Develop a simulation environment that replicates the real-time data we observe.
  - We estimate this will require 3 weeks and sub-tasks will be fleshed out in weekly updates
2. Develop and test multiple algorithms that choose a subcontractor
  - We estimate this will take 6 weeks and sub-tasks will be fleshed out in weekly updates
3. Develop a benchmark that shows how well a particular algorithm performs
  - We estimate this will take 0 weeks as it will be a component of (2)
4. Roll out the algorithm in production environment
  - We estimate this will take 2 weeks and sub-tasks will be fleshed out in weekly updates


## Deadlines

**January 6, 2025**: Initial simulation environment live and tested

**January 20, 2025**: Test at least one algorithm in the simulation environment

**February 3, 2025**: Develop evaluation metric for the simulation environment

**February 17, 2025**: Develop and test at least two additional algorithms

**February 24, 2025**: Write up results and check in with shareholders

**March 3, 2025**: Use feedback to evaluate whether additional algorithms needed

**March 10, 2025**: Begin testing algorithms in production environment

