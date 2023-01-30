# PART 1 - SERVERS
<img width="611" alt="image" src="https://user-images.githubusercontent.com/122497642/215369140-d2c50061-807d-4284-bbd8-0b60fcfce2a8.png">

<img width="441" alt="image" src="https://user-images.githubusercontent.com/122497642/215369213-c389435f-5c77-4a7c-8bbe-e9a1dcc3f239.png"> 

This screenshot called the main method in the StringServer class and the handleRequest method in the Handler class. Main took in what was passed in the command terminal, including the port number, while handleRequest took in the url, with the string message. The webpage presented all the string messages passed in while the server was still running, and created a new line between each string message.


    
<img width="441" alt="image" src="https://user-images.githubusercontent.com/122497642/215369309-1b8fbb7c-80b0-4cd5-8bfa-fcd5e8a8a442.png"> 

This screenshot called the main method in the StringServer class and the handleRequest method in the Handler class. The same things from the previous screenshot happened in this screenshot, except I passed in numbers as messages in the url, but the code and webpage still took that in as string.

# PART 2 - BUGS
### Failure-inducing input

The JUnit test
```
  @Test
  public void testReversed1() {
    int[] input1 = {4, 5, 6, 7 , 8, 9};
    assertArrayEquals(new int[]{9, 8, 7, 6, 5, 4}, ArrayExamples.reversed(input1));
  }
  
 ```
  
  ### Non-failure-inducing input
  
  The Junit test
  ```
  @Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
  ```
  
### The symptom
<img width="585" alt="image" src="https://user-images.githubusercontent.com/122497642/215415669-b9422412-f506-45b9-975c-52dfff2479eb.png">


### The bug
 The code before
 ```  
 static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
  ```
  
  The code after
  ```
    static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
  ```
The bug was that the old code had the normal initialized array become updated with whatever was in newArray, but newArray was null. Therefore, array wasn't being updated properly, so it remained the same, since array was returned. To fix this, I swapped in the for loop and return array with newArray, so newArray holds the reversed values of array and is returned, so the program displays the reversed array.


# PART 3 - SOMETHING NEW
From the lab sessions these past two weeks, I learned howa url works and how to manipulate it. I  was able to create my own web server, with a custom url that displayed unique messages. It was really interesting to see the process of developing a web server with custom requests.
  
