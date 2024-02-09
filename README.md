# Maximum-Number-Using-Digits
You have a set of digits, and your goal is to create the largest possible integer using all these digits. However. there are specific rules:     The integer you create must be divisible by 2 and 5 without any remainder.  You can use any of the digits in the set, but you cannot use leading zeroes 

def find_max_integer(n, digits):
    if 0 not in digits:
        print("-1")
        return

    digits.sort(reverse=True)

    if digits[0] == 0:
        print("0")
        return

    result = int("".join(map(str, digits)))
    print(result)

n = int(input())
digits = list(map(int, input().split()))

find_max_integer(n, digits)
