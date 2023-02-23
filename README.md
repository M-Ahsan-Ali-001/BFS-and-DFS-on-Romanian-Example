# BFS-and-DFS-on-Romanian-Example
# library Used
1.) networkx
2.) matplotlib
3.) queue

# Explanation
1.) In this task I have created two option in which user can manually enter cities and thier neighbours with their weight and user have also option to automatically generated this data.

2.) After taking the input from user, I have created two classes **path_recovery** and **graphF** , path_recovery class finds the  correct route and cost of both BFS and DFS , graphF class has constuctor to intialize the Queue **self.frontier**, two lists (**self.frontierDfs** , **self.explored**).

3.) **graphF** class has two function **BFS** and **DFS**, in BFS we first create a new node of class **path_recovery** and than we will push start and and new node as a tuple to frontier stack.

4.) Now(BFS continued), I have used a loop to  itreate until Queue **self.frontier** is empty, in this loop , I have  popped tuples in FIFO manner() and stored them in two varaibles. after that I have used conditional statement to check if the city is equal to goal ( basically goal and start is a variable which shows where to start and end the route), in that statment I have returned the path_recovery object  and printed the result and the cost, after that there is another if statement in which  I have checked ** if city is not in the explored list nad city is not equal to goal**, if it's true I have created new path_recovery node added previous node data and current city name and cost(It helps in storing the correct sequence and finding cost).

5.) When Queue **self.frontier** becomes empty, correct path and cost of **BFS** will be printed on the screen.


6.) In DFS , I have used a loop to  itreate until List **self.frontierDfs** the length become zero, in this loop , I have  popped tuples in LIFO manner() and stored them in two varaibles. after that I have used conditional statement to check if the city is equal to goal ( basically goal and start is a variable which shows where to start and end the route), in that statment I have returned the path_recovery object  and printed the result and the cost, after that there another if statement in which we I have checked ** if city is not in the explored list nad city is not equal to goal**, if it's true than I have created new path_recovery node added previous node data and current city name and cost(It helps in storing the correct sequence and finding cost).

7.) When Queue **self.frontierDfs** becomes empty, correct path and cost of **DFS** will be printed on the screen.


# BFS & DFS result Comparison
~~~
goal Reachead!
Path Route: ['Arad', 'Sibiu', 'Fagaras', 'Bucharest']
Cost : [211, 99, 140, 0]  Total: 450
goal Reachead!
Path Route: ['Arad', 'Timisoara', 'Lugoj', 'Mehadia', 'Drobeta', 'Craiova', 'Pitesti', 'Bucharest']
Cost : [101, 138, 120, 75, 70, 111, 118, 0]  Total: 733
BFS has out-perfomed the DFS
~~~
From above senario we can say that, **BFS has out-perfomed the DFS.**

# Visual Representation

![image](https://user-images.githubusercontent.com/91987110/220993585-66168394-00e0-440a-9872-db2e307d4d8e.png)

![image](https://user-images.githubusercontent.com/91987110/220993714-1398739c-7c61-4613-9ef3-e0d2fb3ef917.png)




