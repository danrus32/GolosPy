import pyttsx3
from tkinter import *
import time

def golos(inputn):

          
        if (inputn == ""):
            inputn ="Lead the text first:"
        golos = pyttsx3.init()
        voices = golos.getProperty('voices')
        if (selected.get() == 1):
            golos.setProperty('voice',voices[0].id)
        elif (selected.get() == 2):
            golos.setProperty('voice',voices[1].id )
        else :
            golos.setProperty('voice',voices[2].id)

        
        golos.say(inputn)
        golos.runAndWait()
def pereobrazovati(): 
    try:

        time.sleep(int(txt1.get()))
    except :
        pass
    golos(txt.get())
    lbl1.configure(text= txt.get()) 
    txt.delete( END) 
window = Tk() 
window.title("GolosPY")  
selected = IntVar()    
rad1 = Radiobutton(window,text='Russian', value=1, variable=selected)  
rad2 = Radiobutton(window,text='English woman', value=2, variable=selected)  
rad3 = Radiobutton(window,text='English male', value=3, variable=selected)


 
lbl = Label(window, text="Lead the text:", font=("Arial Bold", 20), width=10)  
btn = Button(window, text="Start!", bg="black", fg="red",command = pereobrazovati,width=10)
txt = Entry(window,width=100) 
txt1 = Entry(window,width=10) 
lbl1 = Label(window, text="")
lbl2 = Label(window, text="Pause after input:")
lbl.grid(column=0, row=0) 

txt.grid(column=0, row=1)  
lbl2.grid(column=0, row=6) 
txt1.grid(column=0, row=7) 
btn.grid(column=0, row=2)
lbl1.grid(column=0, row=8) 

rad1.grid(column=0, row=3)  
rad2.grid(column=0, row=4)  
rad3.grid(column=0, row=5) 
window.geometry('600x600') 
window.mainloop()

