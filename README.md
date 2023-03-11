# python-programme for printing next date
a=int(input("enter the year"))

if a%400==0:
    leap_year=True
elif a%4==0 and a%100!=0:
    leap_year=True
else:
    leap_year=False
    
b=int(input("enter the month"))

if b==2:
    if leap_year:
        c=29
    else:
        c=28
elif b==1:
        c==31
elif b==2:
        c==28
elif b==3:
        c==31
elif b==4:
        c==30
elif b==5:
        c==31
elif b==6:
        c==30
elif b==7:
        c==31
elif b==8:
        c==31
elif b==9:
        c==30
elif b==10:
        c==31
elif b==11:
        c==30
elif b==12:
        c==31
c=int(input("enter the day"))
if (b==12and c==31):
    a=a+1
    c=1
    b=1
else:
    c=c+1
    
print("THe next date is ",(a,b,c))
