'''
#Code below counts the number of charater 'a'
nline=0
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    nline=nline+1
print(nline)
'''

'''
#Code below prints mytext.txt line by line
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    print(line)
'''

#Code below prints mytext.txt line by line without right whitespace
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    print(line.rstrip())

#Code below counts and prints the number of charaters in each line including spaces.
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    right_space_removed_line=line.rstrip()
    ncharacters_in_line=len(right_space_removed_line)
    print(ncharacters_in_line)

#Code below counts and prints the number of charaters in each line except spaces.
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    right_space_removed_line=line.rstrip()
    ncharacters_in_line=len(right_space_removed_line)
    print(ncharacters_in_line-right_space_removed_line.count(' '))

#Code below counts and prints the number of a-charaters in each line.
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    right_space_removed_line=line.rstrip()
    nacharacters_in_line=right_space_removed_line.count('a')
    print(nacharacters_in_line)

#Code below counts and prints the number of a and A-charaters in each line.
file_object=open('mytext.txt','r',encoding='utf-8')
for line in file_object:
    right_space_removed_line=line.rstrip()
    nacharacters_in_line=right_space_removed_line.lower().count('a')
    #nacharacters_in_line=right_space_removed_line.replace(A,a).count('a')
    print(nacharacters_in_line)


#Test example for whiteapce
line1_string='text1'
line2_string='text2'
print(line1_string)
print(line2_string)

line1_string='text1\n'
line2_string='text2'
print(line1_string)
print(line2_string)

line1_string=line1_string.rstrip()
print(line1_string)
print(line2_string)

#Code below prints odd numbers lesser than 10
n=0
while n<10:
    n=n+1
    if n%2==0:
       continue
    print(n)


#Code below receives input and calculates the sum and average
count=0
sum_of_nums=0
while 1==1:
    my_input=input()
    if(my_input=='done'):
        break
    my_input=float(my_input)
    sum_of_nums=sum_of_nums+my_input
    count=count+1
mean=sum_of_nums/count
print('sum:',sum_of_nums)
print('mean:',mean)

#Calculate remainder of x / y
def remainder(x,y):
    return x%y

print(remainder(17,3))
