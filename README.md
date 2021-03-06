# design-patterns

-----------------------------------------------------------------------------------------------------------------------------------------------
### Laboratory Work 1

It was done in a form of a fantasy game and where the following design patterns were implemented:

- Factory pattern -> <font color='green'>tavern_factory.py</font>
  
  Code:
  
  ![image](https://user-images.githubusercontent.com/55151032/142234147-9dd4d7ce-7e94-4684-a4f6-63ffe535f383.png)

  In case of Factory pattern, I decided to implement it independently and in such a way it representes one of the 
  possible paths that the main character can take 'Tavern', that comes with some kind of consequences.
  
- Abstract factory pattern -> <font color='green'>sword_factory_method.py</font>

  In abstract pattern was implemented the basic logic of world creation, with 2 main stories depending on the 
  character type.
 
- Builder pattern -> <font color='green'>charcater_builder.py</font>

Console output:

![image](https://user-images.githubusercontent.com/55151032/142233694-96a8e5e4-f527-44e5-a18b-dd15dd19afb0.png)

-----------------------------------------------------------------------------------------------------------------------------------------------
### Laboratory Work 2

For this laboratory work I decided to implement the following design patterns from the list provided:

- #### Adapter pattern
  
  Adapter method was implemented inside a class, by manipulatinf 2 other classes that is basically an
  implementation of Factory design pattern. 
  
  ![image](https://user-images.githubusercontent.com/55151032/142229971-b585b8b9-7a46-46fb-8ebb-d6bca1897921.png)
  
  Here we have 2 different classes of monsters that both have a method of attack, but due to their different
  specialities, we can consider using different names for this methods, in such a way we use the Adapter method
  to get a more comfortable way of using this both classes simultaneously. The class 'MonsterSpawn' is called in
  the file 'abstract_factory.py' from the previous laboratory work
  
  Console output:
  
  ![image](https://user-images.githubusercontent.com/55151032/142233562-1c67c9b9-5d83-4891-9e99-b78dee9fa8d0.png)

- #### Decorator pattern

  Decorator pattern was implemented superficially, but it shows the basic idea behind this type of 
  pattern.
  
  ![image](https://user-images.githubusercontent.com/55151032/142229498-43e68083-3c30-4527-892e-f9be13b78085.png)
  
  ![image](https://user-images.githubusercontent.com/55151032/142229553-8e30fcc9-09a2-4615-84d3-468d77fa1432.png)
  

- #### Proxy pattern - protection proxy;

  Proxy pattern was implemented independently from the general laboratory work, and represents
  a new feature in the improvised game a 'Bag' that holds different types of materials. The proxy 
  approach is observed and is represented by the fact that it is impossible to change the materials
  of the bag without the knowledge about the secret key.
  
  ![image](https://user-images.githubusercontent.com/55151032/142227946-294fb33a-4bec-48c1-b126-038e33838648.png)
  
  Even, if this code has a big security flaw, because of the password being stored in the source code and being
  stored as plain text this can serve as an example only.
  
  Console output:
  
  ![image](https://user-images.githubusercontent.com/55151032/142233208-3f237123-7866-4d64-bd07-50944c8caec4.png)

-----------------------------------------------------------------------------------------------------------------------------------------------
### Laboratory Work 3

- #### Strategy pattern
  
  The Strategy pattern promotes using multiple algorithms to solve a problem. Its killer feature is that it makes it possible to switch algorithms
  at runtime transparently.
  
  ![image](https://user-images.githubusercontent.com/55151032/144117227-c762ab2d-59ee-4201-871a-946b3f219a8a.png)
  
  Here we can observ 2 different methods, for 2 types of situation depending on the class of the character chosen. In such a way we can
  add even more strategies, for different situations for a better control and ensuring a better game experience.
  
  ![image](https://user-images.githubusercontent.com/55151032/144117461-59f9c084-4f4a-453c-8d25-35702dddd7f7.png)
  
  The strategy pattern was implemented in a form of class, and strategies are methods of this class. Also, above we can see the method that controls 
  the general logic of the class, and in order to activate new strategies a change in this method is required. The complete code can be found in 
  'Lab3.py' file, and is integrated in the abstract factory method from Laboratory Work Nr.1.
