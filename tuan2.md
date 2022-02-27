# **Array**

- ### Create array
- ### Process array
- ### Foreach loops
- ### Passing Array to Methods
- ### Return Arrays form Methods
- ### Arrays class

## 3. **Passing Array to Methods**

### Cấu trúc để truyền mảng vào phương thức

```java:
method_name(array):
```

Trong đó :

_method_name_ là phương thức chúng ta cần truyền giá trị của mảng vào.

_array_ là mảng cần truyền vào phương thức.

Ví dụ

```java:
public static int[] Sum(int[] array){
    int Sum = 0;
    for(int i = 0; i < array.length ;i++){
        Sum += array[i];
    }
    return Sum ;
}

```

```java:
public static void main(Stirng[] args){
    int[] demo = {1,2,3,10,2,5,23};
    //Cách 1:
    System.out.println("Sum = " + Sum(demo));
    //Cách 2
    System.out.println("Sum = " + Sum(new int[]{10,20,30,40,50,60,70,80}));
}
```

## 4. **Return an Array from a Method**

Chúng ta có thể trả về giá trị của mảng từ phương thức

VD:

```java:
import java.util.*;
public class Main
{
public static String[] return_Array() {

       String[] ret_Array = {"Java", "C++", "Python", "Ruby", "C"};

      return ret_Array;
   }

public static void main(String args[]) {

     String[] str_Array = return_Array();
     System.out.println("Array returned from method:" + Arrays.toString(str_Array));
    }
}
```

## 5. **Array class**

Để sử dụng lớp Array chúng ta cần khai báo lớp :

```java:
import java.util.Arrays;
```

Cú pháp để sử dụng các phương thức trong lớp Arrays:

```
Arrays.<function name>;
```

Các phương thức trong lớp Arrays:

- toString()
- sort()
- binarySearch()
- ...

## Methods toString()

Dùng để hiển thị tất cả các phần tử trong mảng

```java:
 public class toString{
     public static void main(String[] args){
         int[] array = {5,7,2,7,14,34,1};
         System.out.println(Array.toString(array));

     }
 }
```

## Methods sort()

Dùng để sắp xếp các phần tử theo thứ tự tăng dần

Phương thức này dùng Quicksort

```java:
 public class sort{
     public static void main(String[] args){
         int[] array = {5,7,2,7,14,34,1};
         Array.sort(array);
         System.out.println(Array.toString(array));

     }
 }
```

## Methods binarySearch()

Phương thức binarySearch() được sử dụng để tìm vị trí của phần tử trong mảng bằng phương thức tìm kiếm nhị phân (binary search). Các phần tử trong mảng phải được sắp xếp trước khi gọi phương thức này.

```java:
 public class binarySearch{
     public static void main(String[] args){
         int[] array = {5,7,2,7,14,34,1};
         Array.sort(array);
         System.out.println(Array.toString(array));

     }
 }
```
