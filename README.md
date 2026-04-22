import tkinter as tk


def add1 ():
    num1 = int(label1.get())
    num2 = int(label2.get())
    b = num1 + num2
    label3.delete(0, 'end')
    label3.insert(0, b)
def add2 ():
    num1 = int(label1.get())
    num2 = int(label2.get())
    b = num1 - num2
    label3.delete(0, 'end')
    label3.insert(0, b)
def add3 ():
    num1 = int(label1.get())
    num2 = int(label2.get())
    b = num1 / num2
    label3.delete(0, 'end')
    label3.insert(0, b)
def add4 ():
    num1 = int(label1.get())
    num2 = int(label2.get())
    b = num1 * num2
    label3.delete(0, 'end')
    label3.insert(0, b)

root = tk.Tk()
root.title('калькулятор')
root.geometry('160x250')

text1 = tk.Label(root, width = 20, text = 'введите первое число')
text1.place(x = 0, y = 30)
label1 = tk.Entry(root, width=25)
label1.place(x=0, y = 50)

text2 = tk.Label(root, width = 20, text = 'введите второе число')
text2.place(x = 0, y = 80)
label2 = tk.Entry(root, width=25)
label2.place(x=0, y = 100)

batton1 = tk.Button(root, width = 3, height = 3, text = '+', command = add1)
batton1.place(x = 0, y = 130)
batton2 = tk.Button(root, width = 3, height = 3, text = '-', command = add2)
batton2.place(x = 35, y = 130)
batton3 = tk.Button(root, width = 3, height = 3, text = '/', command = add3)
batton3.place(x = 70, y = 130)
batton4 = tk.Button(root, width = 3, height = 3, text = '*', command = add4)
batton4.place(x = 105, y = 130)

text3 = tk.Label(root, width = 20, text = 'введите первое число')
text3.place(x = 0, y = 195)
label3 = tk.Entry(root, width=25)
label3.place(x=0, y = 220)

root.mainloop()
