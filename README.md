import math
print('一元二次方程，ax^2+bx+c=0 求解程序')

a = input('请输入a的值：')
b = input('请输入b的值：')
c = input('请输入c的值：')
a = float(a)
b = float(b)
c = float(c)
u =b*b
i = 4*a*c
su = float(u)
sa = float(i)
if su<sa:
    print('此方程无实数解')
elif su==sa:
    x = -b/2/a
    print(x)
else:
    xa = (-b+math.sqrt(b*b-4*a*c))/2/a
    xb = (-b-math.sqrt(b*b-4*a*c))/2/a
    print('此方程的解为x1=%s\n x2=%s' %(xa,xb))
