
**Determine time complexity for below problems:**

1. 
```*.java

void foo(int[] array){
  int sum = 0;
  int product = 1;
  for(int i=0; i < array.length; i++) {
    sum += array[i];
  }
  
  for(int i=0; i < array.length; i++) {
    product *= array[i];
  }
  
  System.out.println(sum + ", " + product);
}

```

Answer: 


2. 
```*.java

int binarySearch(int arr[], int l, int r, int x)
{  
  if (r>=l)
    {
      int mid = l + (r – l)/2;

      if (arr[mid] == x)

      return mid;

      if (arr[mid] > x)

      return binarySearch(arr, l, mid-1, x);

      return binarySearch(arr, mid+1, r, x);
    } 
  return -1;
}

```

Answer: 

3. 
```*.c

#include <stdio.h> 
void main() 
{ 
    int i, n = 8; 
    for (i = 1; i <= n; i++) { 
        printf("Hello Word !!!"); 
    } 
} 

```

Answer: 

4. 
```*.c

#include <stdio.h> 
void main() 
{ 
    int i, n = 8; 
    printf("Hello Word !!!"); 
} 

```

Answer: 

5. 
```*.c

#include <stdio.h> 
void main() 
{ 
    int i, n = 8; 
    for (i = 1; i < n; i = i * 2){
      printf("Hey - I'm busy looking at: %d", i);
    }
} 

```

6.

```*.java
for (int i = 1; i <= n; i++){
    for(int j = 1; j < 8; j = j * 2) {
        System.out.println("Hey - I'm busy looking at: " + i + " and " + j);
    }
}
```

Answer: 

7.

```*.java

for(int j = 1; j <= n; j++) {
    System.out.println("Hey - I'm busy looking at: " + i + " and " + j);
}

for (int i = 1; i <= n; i++) {
    for(int j = 1; j <= n; j++) {
        System.out.println("Hey - I'm busy looking at: " + i + " and " + j);
    }
}
```

Answer: 

6.

```*.java
for (int i = 1; i <= n; i++) {
    for(int j = 1; j <= n; j++) {
        for(int k=0; k <= n; k++) {
          System.out.println("Hey - I'm busy looking at: " + i + " and " + j + " and " + k);
        }
    }
}
```

Answer: 

7.

```*.java
for (int i = 1; i <= Math.pow(2, n); i++){
    System.out.println("Hey - I'm busy looking at: " + i);
}
```

Answer: 

8.

```*.java
int fib(int n) 
{ 
  if (n <= 1) 
     return n; 
  return fib(n-1) + fib(n-2); 
} 
```

Answer: 

9.

```*.java
public static void printFirstItemThenFirstHalfThenSayHi100Times(int[] items) {
    System.out.println(items[0]);

    int middleIndex = items.length / 2;
    int index = 0;

    while (index < middleIndex) {
        System.out.println(items[index]);
        index++;
    }

    for (int i = 0; i < 100; i++) {
        System.out.println("hi");
    }
}
```

Answer: 


**Can you answer out of all the above programs, which one has the worst time complexity and which one has the bext?
Write the program number and it's complexity**

Answer:
- Worst:
- Best: 


**Common Big-O functions:**
- O(1) - constant time
- O(log(n)) - logarithmic time
- O((log(n))c) - polylogarithmic time
- O(n) - linear time
- O(n2) - quadratic time
- O(nc) - polynomial time
- O(cn) - exponential time
- O(n!) - factorial time

Refer https://www.bigocheatsheet.com/ to know what is worst
