### APPLICATION-PROGRAMMING-II-ASSIGNMENT

##### SCT221-C002-0011/2021
#### Quresho Mohamed 
#### APPLICATION PROGRAMMING II ASSIGNMENT
#### Question one


Write a program that will assign a random number to the variable n each time it is executed. Complete the source code to print whether the number stored in the variable n is positive or negative.

``` Imports System
    Module Module1
      Sub Main() 

      Dim random As New Random()
        Dim n As Integer = random.Next(-1, 1) 
        If n > 0 Then
            Console.WriteLine("The number {0} is positive.", n)
        ElseIf n < 0 Then
            Console.WriteLine("The number {0} is negative.", n)
        Else
            Console.WriteLine("The number is zero.")
        End If
    End Sub
End Module
```
#### Question two
This program will assign a random number to the variable n each time it is executed. Complete the source code to print the last digit of the number stored in the variable n.

```
Imports System
Module Program
    Sub Main(args As String())
        Dim rand As New Random()
        Dim n As Integer = rand.Next(0, 1000)
        Console.WriteLine(n Mod 10)
    End Sub
End Module
```

#### Question Three
Write a function that swaps the values of two integers.

```
Imports System
Module Program
    Sub Main(args As String())
        Dim a As Integer = 7
        Dim b As Integer = 12
        Console.WriteLine("Before swapping, a = " & a & " and b = " & b)
        a = a Xor b
        b = a Xor b
        a = a Xor b
        Console.WriteLine("After swapping, a = " & a & " and b = " & b)
    End Sub
End Module
```

#### Question Four
Write a function that prints a string, followed by a new line.

```
Module Module1
Sub Main()
 Dim message As String = "Hello, world!"
Console.WriteLine(message)
End Sub
End Module
```

#### Question Five
Write a function that prints a string in reverse.

```
Module Module1
 Sub Main()
Dim originalString As String = "Hello, world!"
Dim words() As String = originalString.Split(" "c)
Array.Reverse(words)
Dim reversedString As String = String.Join(" ", words)
Console.WriteLine(reversedString)
End Sub
End Module
```

#### Question six
Write a function that gets the length of a prefix substring

```
Module Module1
Sub Main()
Dim originalString As String = "Hello, world!"
Dim prefix As String = "world"
Dim prefixLength As Integer = Len(prefix)
Dim prefixSubstring As String = originalString.Substring(0, prefixLength)
Console.WriteLine(prefixSubstring)

End Sub
End Module
```
