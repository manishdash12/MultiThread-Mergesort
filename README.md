# Multi Threading in Java
In this project we explore the multi-threading libraries of Java. We wanted to implement **Merge Sort using Recursive Action and ForkJoin principle** using the said multi-threading libraries. 

The project is a search application, that takes a query string as input and searches it in all the text files located in the **Input** folder.

Different threads open and search files for the query and outputs a **score** based on its location in the file. A sorted list of all search results based on the score is given as output, which is stored in **output.txt**. The two ways of doing it are explored and mentioned as Implementation One/Two.

* **Implementation One**: Uses traditional ways of creating threads, like use of runnable and 
```
			Thread t = new Thread(new ObjectOfTask);
```


* **Implementation Two**: Uses Executor Services to create a thread pool, also uses Callable instead of runnable 
```
			ExecutorService executor = Executors.newFixedThreadPool(numThreads);
```

Apart from this, forkJoin principle is used to implement MergeSort in a distributed multi threaded fashion. 

