# set-operations
# write a prog. that generates a set of prime no's and another set of odd numbers .Demonstrate the result of union , intersection , difference and assymmetric difference operations on these sets.
odd=set([x*2+1 for x in range(1,10)])
print(odd)
prime=set()
for i in range(2,20):
    j=2
    is_prime=True
    while j<=i//2:
        if i%j==0:
            is_prime=False
            break
        j+=1
    if is_prime:
        prime.add(i)
print(prime)
