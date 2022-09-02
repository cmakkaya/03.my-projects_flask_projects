from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def head():
    return render_template('index.html', number1 = 7000, number2 = 9000)







if __name__ == '__main__':
    app.run(debug=True)