# Input the X, The function will return prime elements of the X
# ZEFiX 9.13.2022


def prime_elements(X):
    
    def primes_until_number(input_number): # It will find a list of primes numbers those the number is dividable by them
        list_of_dividable_primes_by_number = [] 
        for number in range(input_number+1,1,-1):
            if number >= 2 :
                IsPrime = True
                for counter in range (2 ,number):
                    if (number%counter) == 0:
                        IsPrime = False
                if IsPrime :
                    list_of_dividable_primes_by_number.append(number)
        
        return list_of_dividable_primes_by_number


    if X == 1: # Maths' Rule
        print("Invalid")
        quit()
    abs_number = abs(X)
    the_primes = sorted(primes_until_number(abs_number))
    prime_elements = []
    while abs_number > 1: # Finds prime elements
        for prime_number in the_primes:
            if abs_number%prime_number == 0:
                prime_elements.append(str(prime_number))
                abs_number = abs_number/prime_number
    # Out put
    output = sorted(prime_elements)
    output = '*'.join(output)
    if X > 0:
        print(output)
    elif X == 0:
        print(X)
    else:
        print('-1*',output,sep='')
