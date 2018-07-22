Add your answers to the Algorithms exercises here.

a) O(n^3)
b) O(n)
c) O(64 * sqrt(n)/2) => O(sqrt(n))
d) O(n * sqrt(n))
e) O(10n^3) => O(n^3)
f) O(n)
g) O(n)

Exercise 2:
a)
    def max_value(a):
        length = len(a)
        big = a[0]
        small = a[0]
        for i in range(length):
            if a[i] > big:
                j = i
                big = a[i]
            else:
                continue
        for i in range(j):
            if a[i] < small:
                small = a[i]

        return big - small
b)
    First, drop an egg from the middle floor (f/2). If the egg breaks, then half the bottom half of the floors ((f/2)/2 == f/4) and drop from that height to see if the egg breaks. If the egg doesn't break, then drop an egg from the midpoint of the top half of the building (3/4 f) to see if it does or doesn't break. Keep following this logic until you've found the lowest floor that the egg breaks from.+

Exercise 3:
    a) O(n^2)
    b) O(nlog(n))