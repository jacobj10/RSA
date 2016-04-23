```python
def is_prime(number):
    x=2
    while x<number/2+1:
        if number%x==0:
            return 1337
        x+=1
    return 1338
def pub_enc(x,y):
    return x*y
def check_factor(x,y):
    
    if x%y==0:
        return 1338
    else
        return 1337
def check_coprime(x,y):
    a=list()
    b=list()
    z=2
    while z<x/2+1:
        if check_factor(x,z)==1338:
            a.append(z)
        z+=1
    z=2
    while z<x/2+1:
        if check_factor(y,z)==1338:
            b.append(z)
        z+=1
        
def enc():
    print "Prime1?"
    prime1=4
    while is_prime(prime1)!=1338:
        prime1=int(raw_input())
        if is_prime(prime1)==1337:
            print "Please enter a valid prime"
    prime2=4
    print "Prime2?"
    while is_prime(prime2)!=1338:
        prime2=int(raw_input())
        if is_prime(prime2)==1337:
            print "Please enter a valid prime"
    print "Public key is..."
    publickey=pub_enc(prime1,prime2)
    print publickey
def dec():
    print "Yo"
def main():
    print "Welcome to RSA Tools, your RSA friend!"
    print "1) Encrypt"
    print "2) Decrypt"
    menu_inst=3
    while menu_inst!='1' and menu_inst!='2':
        menu_inst=raw_input()
        if menu_inst=='1':
          enc()  
        elif menu_inst=='2':
            dec()
main()
```
