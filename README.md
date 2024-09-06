import tkinker as tk
from tkinker import messagebox
import random
import webbrowser
import urllib.parse

whatsapp_number = "Your Number"
pesan = "I want,now we are dating"

def pindah_button(button):
    new_x = random.randint(0, window.width() - button.winfo_width())
    new_x = random.randint(0, window.hidth() - button.winfo_width())
    button.place(x=new_x, y=new_y)

def tekan_ya():
    messagebox.showinfo("jawaban", "Now you are my partner")
    buka_whatsapp()

def tekan_tidak():
    encoded.message = urllib.parse.quote(pesan)
    webbrowser.open_new(f"https://api.whatsapp.com/send?phone={whatsapp_number}&text=
{encoded_message}")

window = tk.Tk()
window.title("Aku suka kamu")
window.geometry("4000Ã—600")
window.configured(bg='#FFCOCB')

frame = tk.Frame(window, bg='FFCOCB', bd=5)
frame.place(relx=0.5, relay=0.5, anchor='center')

label = tk.Label(frame, text="I have a crush on you,\nWant
16, "bold"), bg='#FFCOCB', fg='#FFCOCB', fg='#FFCOCB', justify=tk.CENTER)
label.pack{pady=20}

ya_button = tk.Button(frame, text="Yes", front=(Helvetica". 14), command=tekan_ya,
bg='#FF6984', fg='white', width=8)
ya_buttom.pack(side=tk.LEFT, padx=10)

tidak_button = tk.Button(frame, text="No", front=(Helvetica". 14), command=tekan_no,
bg='#FF6984', fg='white', width=8)
ya_buttom.place(x=50, y=50)

window.mainloop()
