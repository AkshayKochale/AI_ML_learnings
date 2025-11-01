
<h1 style="color: #cdc60bff">  Probability </h1>

- Probability in simple words is what are the chances of particular event happening

- Example 
    - Consider dice from number (1 to 6) what are the chances of getting odd number on each throw
    
    - Here numbers {1,2,3,4,5,6} are consider as Sample space

    - Numbers {1,3,5} are events

    - Formula is (number of events) / (number of sample space) which is 3/6 or 0.5

    - So in percentage(%) we have 50% of chance getting odd number 


## Mathmatical sets for probability 

- Set in are some list object where each element is unique

- Example
    - We have sample student set (universal set in terms of set) as U = {s1,s2,s3,s4,s5,s6....s100}
    
    - Also we have 2 different set 
        - Student who learn computer science as cs = {s2,s5,s6} 
        - Student who learn math are m = {s1,s2,s3,s4,s6,s55}

    - Let 'N' be total number of student hence we can say
        - N(U) => Total number of student
        - N(cs) => Total cs student
        - N(m) => Total math student

    - Calculations    
        - now we can say N(total student with both subject) = N(cs) ∩ N(m) = {s2,s6} # Intersection
        - N(total studen who are stuying either of subject) = N(cs) + N(m) - (N(cs) ∩ N(m)) # union
        - which will be N(cs U m) = {s1,s2,s3,s4,s5,s6,s55}
        - Note : why we need to remove intersection ? as there are common student who learn both are counted, student who study math also study cs
        - N(cs ∩ m) ⊆ N(cs U m) ⊆ N(U)

<br>
<p align="center">
  <img src="./Images/SetExample.png" alt="Student Sets Venn Diagram" width="500"/></p>




## What are fair events?

 - suppose we have coin and we tossed it then either we can get heads or tails
 - So the probability of getting heads is P(h)
 - if coin is tossed 10 times then in most cases 4 to 6 head 
 - similary if we toss for 100 then close to 50 , 1000 then close to 500 (Most of the time)
 - here chances of getting heads are close to 0.5 or 50% , hence this types of events are fair events



## Joint probability 

 - With given sample set 2 or more  events occure at same time
 - Example 
    1. <b>Suppose we have given a fair dice ,and we need to find probability of event where number is even, prime and odd ?</b>
    - So sample set(U) = {1,2,3,4,5,6}
    - even event (A) = {2,4,6}
    - prime event (B) = {2,3,5}
    - odd event (C) = {1,3,5} 
    - we need to find P(A and B and C) which can be represent as P(A ∩ B ∩ c) which is Empty set {},
    as, no elements are common 
    
    2. <b>Similarly find probabilty of event where number is prime or even ?</b>
    - here we need to find P(B or C) which can be represent as P(B U C) = {2,3,4,5,6} 


## Conditional probability

  -  Probability of certain event based on another condition
  - Example 
     1. <b>What is probability of getting prime number which are even?</b>
        -  So  P(X)={2} , here X is prime number which are even 
        - In this case there are probability of certain event based on some condition 
        - Which is denoated by P(X)=P(A | B) , where A is prime number and B is even
        - we can say that P(X) = P(A ∩ B ) / P(B) 
        - P(A ∩ B) = { 2 }  and P(B)={2,4,6} hence answer is 1/3 = 0.33



## Types of events?

- Mainly there are 2 major types of event

 1. <b>Mutual exclusive event</b>
    - For any two events if one event can exclude another event, in other term only one of the event can occure at any given time is called mutual exclusion events 
    - Given a fair dice 
    - A : {2,4,6}  # even numbers
    - B : {1,3,5}  # odd numbers
    - here A ∩ B is {}, hence P(A ∩ B ) = 0 , so number can be either even or odd, it cannot be both

  2. <b>Independent event </b>
     - For any two events probability of that one event happening is independent of another event 
     - Given a deck of cards
     - A : {4} # probability of gettting 'king' out of 52 card which is (4/52) = 1/13
     - B : {13} # probability of getting 'heart' card which is (13/52) = 1/4
     - P(A | B) : probability of getting 'king with heart' = P(A ∩ B)/P(B) (conditional probability formula) = (1/52) / (1/4) = 4/52 = 1/13
     - hence P(A) = P (A | B) , so we can say that even if card is heart only one of the card will be king and event without heart probability of getting heart is (1/13)
     - this two event are independent as probability does not change on each condition 
