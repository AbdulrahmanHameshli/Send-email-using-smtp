import smtplib
from email.message import EmailMessage

def send_alert(massege, body ,to):
    msg=EmailMessage()
    msg.set_content(massege)
    msg["subject"]=body
    msg['to'] = to
    


    us = "Username"
    msg['from']="from me"
    pw= "Password" 

    server = smtplib.SMTP('smtp.gmail.com', 587)   #smtp:simple mail transfer protocol, 587 is thr port for tls=Transport Layer Security, krypterande meddelande för säkerhet.
    server.starttls()
    server.login(us,pw)
    server.send_message(msg)
    server.quit()

if __name__=="__main__":
    send_alert("Hi bro, somebody is in your home, check the camra","Home allert","to_person")
