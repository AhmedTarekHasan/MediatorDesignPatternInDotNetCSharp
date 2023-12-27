<link rel="canonical" href="https://www.developmentsimplyput.com/post/mediator-design-pattern-in-net-c" />

# Mediator Design Pattern In .NET C#
### Learn about the Mediator Design Pattern in .NET C# with code samples.

<p align="center">
  <img src="https://static.wixstatic.com/media/488a99_0c4ead8ea5704a81a9a48e2e8e0d48ff~mv2.png">
</p>

<br/>

<p>
The Mediator Design Pattern is one of the behavioral design patterns.
</p>

<br/>

<p>
According to Wikipedia, the definition is as follows: The essence of the Mediator Pattern is to “define an object that encapsulates how a set of objects interact”. It promotes loose coupling by keeping objects from referring to each other explicitly, and it allows their interaction to be varied independently. Client classes can use the mediator to send messages to other clients, and can receive messages from other clients via an event on the mediator class.
</p>

<br/>

<p>
Therefore, to put it in simple words, the Mediator Design Pattern is used to manage the interactions between group of objects (similar or not) keeping the the objects isolated from each other.
</p>

<br/>

<p>
To understand this, let me explain more with a simple example.
</p>

<br/>

<p>
Let’s say that you are implementing a Chat Room. So, you have unlimited number of users who can join the room and once any user sends a message, the message should be received by all other users on the Chat Room.
</p>

<br/>

<p>
So, implementing this, you would have a User class with SendMessage method.
</p>

<br/>

<p>
However, you still need to have access to the other Users so that you can direct your the message to them. Also, whenever, a User leaves the Chat Room, you would also need to remove this User from all other Users so that they don’t send a message to him.
</p>

<br/>

<p>
You have more than one way to achieve this:<br/>
1. Defining a list of Users inside each User and keeping these lists updated whenever a User enters or leaves the Chat Room.<br/>
2. Using another class or module to act as the middle man to handle the Users list and the way of sending and receiving the messages between different Users.
</p>

<br/>

If you are interested into reading more about this topic, you can read [the rest of the article][Article]. 

<br/>

## If you want to support me:
▶ Subscribe to Medium using [my referral link][Membership]<br/>
▶ Subscribe to [Medium Newsletter][Subscribe]<br/>
▶ Subscribe to [LinkedIn Newsletter][Newsletter]<br/>
▶ Follow me on [Medium][Blog]<br/>
▶ Follow me on [Twitter][Twitter]<br/>
▶ Follow me on [LinkedIn][LinkedIn]

<br/>

## Authors:
* [Ahmed Tarek Hasan]


[Ahmed Tarek Hasan]: https://medium.com/@eng_ahmed.tarek
[Blog]: https://medium.com/@eng_ahmed.tarek
[Membership]: https://medium.com/@eng_ahmed.tarek/membership
[Subscribe]: https://medium.com/subscribe/@eng_ahmed.tarek
[Twitter]: https://twitter.com/AhmedTarekHasa1
[LinkedIn]: https://www.linkedin.com/in/atarekhasan/
[Friend Links]: https://www.linkedin.com/feed/update/urn:li:activity:6866082670108143616/
[Newsletter]: https://www.linkedin.com/newsletters/development-simply-put-6866647119655247872/
[Article]: https://www.developmentsimplyput.com/post/mediator-design-pattern-in-net-c
