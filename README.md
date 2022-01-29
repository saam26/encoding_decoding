# encoding_decoding

# encoding the given word
word=input("Enter the word:")
d=int(input("Enter the integer"))
List=list(word)
new_word=""
for i in List:
    at=str(i)
    p=ord(at)
    new_char=d+p
    c=chr(new_char)
    new_word+=c
print("The encoded word is ",new_word)

# decoding the given word
List1=list(new_word)
original_word=""
for j in List1:
    bt=str(j)
    k=ord(bt)
    old_char=k-d
    f=chr(old_char)
    original_word+=f
print("The decoded word is ",original_word)
