# Tkinter-Place
Task from https://younglinux.info/tkinter/place
Напишите программу, состоящую из главного окна и кнопки, на которой изображен смайлик. При клике на кнопку она должна оказываться в новом случайном месте окна. Размер окна может меняться.
from tkinter import *
import random
root=Tk()
root.geometry('500x500')
def change_place():
    l.place(relx=random.random())
    l.place(rely=random.random())
img=PhotoImage(file="Min.png")
l=Button(image=img, command=change_place,  bd=3)
l.place(x=0.1,y=0.1)
root.mainloop()
