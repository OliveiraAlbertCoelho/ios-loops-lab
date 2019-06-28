# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**
var i = 1
while i<151 {
print(i)
i+=1
}
***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

var i = 142
for _ in i...157{
i+=1
print(i)
}

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

var i = 15
for _ in i...80{
if i%2==0{

print(i)
}
i+=1

}

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

var i = 19
for _ in i...51{
if i%2 != 0{

print(i)
}
i+=1

}

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**
var i = 1
for _ in i...98{
i+=1
if i%10 == 5{
print(i)
}

}

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**
var i = 1
for _ in i...40{
if i%10 == 7{
print(i)
i+=1
}else{
i+=1
}

}
***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`
var i = 20
while i<=150{
if  i%3==0{
print(i)
i+=1
}else {
i+=1
}
}

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`
var i = 20
while i<=150{
if  i%3==0 && i%2==0 {
print(i)
i+=1
}else {
i+=1
}
}

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`
for eachnum in 20...150 where eachnum % 10 == 4{
print(eachnum)
}

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`
for index in 20...150{
if index == 31 || index == 35{
print(index)
}else if index >= 40 && index <= 60 {
print(index)
    }
}
***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
this is a infinite loop
```

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i <= 9) {
i += 1
}
```

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5
while (i <= 1004) {
i += 1
}

```

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i <= 1004) {
i+=1
if i%2==0 {
print(i)
}

}

```

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
both loops have the same output, the diference between both is that for the while loop to execute a block of code it will check if the statements are true first meanwhile the repeat while loop runs the block of code first and then loops until the condition is false.

```

***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

when break is used in a loop, it ends the loops and whatever code thats outside the loop begins while continue only stops the next lines of code inside the loops, it would go to the next interation.

***
## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10
answer: it would print 1,2,3,8,9,10
***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10
} answer: it would print 1,2,3

***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
the reason for this output is because as soon as the the condition is met for the continue it takes us to the outerloop which does not allow the y loop to run after the value 1
```

***
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.
/ for x in 0...10 {
//     for y in 0...10 {
//        print("x = \(x), y = \(y)")
//        }
//    }
***
## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.
//for x in 0...10 {
//    for y in 0...10 {
//        if x-y==5 || y-x==5{
//         print("x = \(x), y = \(y)")
//    }
//}
//}
***
## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25

var N = 5
var i = 0
while i <= 5{
print(i * i)
i +=  1
}

```

***
## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.
```swift
var num = 5
var asterics = ""
var i = 0
for _ in i..<num {
for _ in i..<num {
asterics += "*"
i+=1
}
print(asterics)
}


***
