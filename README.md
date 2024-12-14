# OE-8

import tkinter as TK

windows = TK.Tk()

name = "Jhusnine Nicole B. Mariano"
windows.title(f"OOP LA30 {name}")
windows.geometry("300x200")
windows.configure(bg="white")

pangalan = TK.Entry(windows)
pangalan.grid(row=0, column=0, padx=20)

counter = 0
def iPrint():
    global counter
    print(f"{counter}.{pangalan.get()}")
    counter +=1

frame = TK.Frame(windows)
frame.grid(pady=20)

button = TK.Button(windows, text="Print", command=iPrint)
button.grid(row=0, column=1, padx=20, pady=20)
windows.mainloop()
