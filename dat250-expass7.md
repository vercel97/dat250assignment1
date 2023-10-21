# DAT250: Software Technology Experiment Assignment 7

## Experiment 1: Installation

RabbitMQ was downloaded via Homebrew, following the following [tutorial](https://www.rabbitmq.com/install-homebrew.html)

![Starting and stopping rabbitMQ](bilder/innlevering7/installing.png)

## Experiment 2: Hello World
In this experiment, a producer that sends one single message and a consumer that recieves messages has been created 
from the code provided in the following [tutorial](https://www.rabbitmq.com/tutorials/tutorial-one-java.html)

Here is the result from running the consumer:
![running the consumer](bilder/innlevering7/exp2.png)

Here is the result from running the producer:
![running the producer](bilder/innlevering7/exp2-2.png)


## Experiment 3: Work Queues
Like in the previous experiment, I have followed the steps in the following [tutorial](https://www.rabbitmq.com/tutorials/tutorial-two-java.html),
this time to create a Work Queue that distributes muoltiple tasks to multiple workers. 

To run the classes in paralell, I edited the run configurations like so:
![](bilder/innlevering7/run-conf.png)

Here is the result from running Round Robin:
![](bilder/innlevering7/exp3-1.png)

![](bilder/innlevering7/exp3-2.png)

![](bilder/innlevering7/exp3-3.png)

![](bilder/innlevering7/exp3-4.png)

![](bilder/innlevering7/exp3-5.png)

## Eperiment 4: Topics
In this experiment the "publish/subscribe" pattern has been implemented following this [tutorial](https://www.rabbitmq.com/tutorials/tutorial-three-java.html).

![](bilder/innlevering7/exp4.png)


### Code 
Here is the code for experiment 1-4:
https://github.com/vercel97/RabbitMQ-experiment.git
