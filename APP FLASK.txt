from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def principal():
    fruta1 = "Morango"
    fruta2 = "Uva"
    fruta3 = "Manga"
    fruta4 = "Banana"

  return render_template("index.html", fruta1=fruta1, fruta2=fruta2, fruta3=fruta3,fruta4=fruta4)
  
@app.route('/sobre')
def sobre():  
    return render_template("sobre.html")
app.run()    
   
#http://127.0.0.1:5000
