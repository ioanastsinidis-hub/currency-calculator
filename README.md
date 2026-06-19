💱 Currency Calculator

A simple and easy-to-use currency conversion tool that allows users to convert amounts between different currencies using exchange rate data.

Whether you're planning a trip, tracking international prices, or just curious about exchange rates, this calculator provides quick and accurate conversions with a clean interface.

✨ Features
Convert between multiple world currencies
Fast and lightweight
Easy-to-understand interface
Supports decimal values
Displays conversion results instantly
Great for learning Python and working with APIs or financial data
📝 Example
Amount: 100
From: USD 🇺🇸
To: EUR 🇪🇺

Result: 100 USD = 92.15 EUR
⚠️ Note

The exchange rate data used in this project may not reflect current market rates and could be outdated. The calculator is intended for educational purposes and basic conversions rather than financial decision-making.

🚀 Why This Project?

This project demonstrates:

User input handling
Mathematical calculations
Working with currencies and exchange rates
Clean program structure
Practical real-world applications of programming

"Money is a terrible master but an excellent servant." — P.T. Barnum 💵<img width="743" height="257" alt="Screenshot 2026-06-08 172010" src="https://github.com/user-attachments/assets/f25aca27-9e57-400d-aa29-8547b8304830" />
code:
from tkinter import *

window = Tk()
window.geometry("600x600")
window.title("metatropeas")
box1= Entry(window)
box1.place(x=50,y=50)
lbl1=Label(window,text="€")
lbl1.place(x=170,y=50)
def somthng():
    money = float(box1.get())
    dolla = money * 1.16
    lbl2.config(text = "$" + str(round(dolla,2)))
    yen = money * 183.98
    lbl3.config(text = "¥" + str(round(yen,2)))
    pound = money * 1.16
    lbl4.config(text = "£" + str(round(pound,2)))
btn1=Button(window, text="->",command=somthng)
btn1.place(x=190,y=50)
lbl2=Label(window, text="$")
lbl2.place(x=220,y=50)
lbl3=Label(window, text="¥")
lbl3.place(x=220, y=65)
lbl4=Label(window, text="£")
lbl4.place(x=220,y=80)
window.mainloop()
