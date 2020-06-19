#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)

n = 3
a less than 3*3*3 27
0 + 9                   1
9 + 9                   2
18 + 9                  3
n=4
a less than 4*4*4 =64
0 + 16                  1
16 + 16                 2
32 + 16                 3
48 + 16                 4
time

b) O(log n)
4 
j = 2     1
j = 4     2

6
j = 2     1
j = 4     2
j = 8     3

25
j = 2     1
j = 4     2
j = 8     3
j = 16    4
j = 32    5

100
j = 2     1
j = 4     2
j = 8     3
j = 16    4
j = 32    5
j = 64    6
j = 128   6

c) I don't know if this is a trick question or just poorly worded. With regards to 'n' this has no runtime complexity because 'n' isn't used. But if you just mean 'n' as a placeholder just like bunnies is a placeholder then runtime complexity is O(n)

bunnies = 5
returns 2+bunnyEars(4)              1
    returns 2+bunnyEars(3)          2
      returns 2+bunnyEars(2)        3
        returns 2+bunnyEars(1)      4
          returns 2+bunnyEars(0)    5
returns 0   

## Exercise II
O(log n)
initiate empty integer called breakfloor
initiate an integer called current floor and set it to n/2
while a condition is false:
    drop an egg from the current floor
        if the egg breaks 
            set the breakfloor to current floor
            subtract one from current floor
        if it doesnt 
            if the current floor is the breakfloor - 1:
                set the condition to true
            set current floor to itself plus 1 floor
return the breakfloor (f)

floor for breaking is 6 (f)
breakfloor = 0 
current floor = 3
condition is false:
    egg doesn't break                                                               1
        curr floor is not 1 less than the breakfloor (which is 0)
            condition is still false
        add one to current floor
        end of while loop, restarts conditional not met
    current floor = 4
    egg doesn't break                                                               2
        curr floor is not 1 less than the breakfloor (which is 0)
            condition is still false
        add one to current floor
        end of while loop, restarts conditional not met
    current floor = 5
    egg doesn't break                                                               3
        curr floor is not 1 less than the breakfloor (which is 0)
            condition is still false
        add one to current floor
        end of while loop, restarts conditional not met
    current floor = 6
    egg does break                                                                  4
        break floor = 6
        conditional still false, do while again
        subtract one from current floor
    current floor = 5
    egg doesn't break                                                               5
        curr floor is 1 less than the breakfloor (which is 6)
            condition is true
    end while loop
return 6 (f)