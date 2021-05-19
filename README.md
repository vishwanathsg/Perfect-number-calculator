# Perfect-number-calculator
This code tells whether a number is perfect, deficient or abundant

#Abundant, deficient & perfect numbers
print()
print("The following program will define every number if they're deficient, abundant or perfect numbers")
print("starting from 2 till the number you're about to enter")

print()

Max=int(input("Enter a positive integer: "))
#User input for a number

Div=1
#Divisor

runner=2
#Start value

while runner<=Max:
    store=0

    while Div<runner:
        if runner % Div==0: #Compund statement
            store=store+Div

        Div=Div+1

    if runner>store:
        print(runner, "is a deficient number") #Suit1

    elif runner==store:
        print(runner, "is a perfect number") #Suit2

    elif runner<store:
        print(runner, "is an abundant number") #Suit 3

    Div=1

    runner=runner+1
