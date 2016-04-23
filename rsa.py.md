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
def totient(x,y):
    return (x-1)*(y-1)
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
    publickey_1=pub_enc(prime1,prime2)
    tot=totient(prime1,prime2)
    print "And your e?"
    e=-1
    while tot%e==0 or e<0:
        e=int(raw_input())
        if tot%e==0 or e<0:
            print "Please enter positive e where e%",tot," does not equal 0"
    
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
