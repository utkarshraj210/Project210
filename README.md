from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return """
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Prem Vivah Bhawan</title>
        <style>
            body { font-family: Arial, sans-serif; text-align: center; margin: 50px; background-color: #f8f8f8; }
            .container { background: white; padding: 20px; border-radius: 10px; box-shadow: 0px 0px 10px rgba(0,0,0,0.1); max-width: 500px; margin: auto; }
            h1 { color: #D81B60; }
            p { font-size: 18px; }
            .contact { margin-top: 20px; font-weight: bold; }
            .contact a { color: #007BFF; text-decoration: none; }
            .contact a:hover { text-decoration: underline; }
        </style>
    </head>
    <body>
        <div class="container">
            <h1>Welcome to Prem Vivah Bhawan</h1>
            <p>Your perfect venue for weddings and celebrations.</p>
            
<div class="contact">
                <p>📞 Call us: <a href="tel:+919279200748">+91 92792 00748</a></p>
                <p>📧 Email: <a href="mailto:utkarshraj27122010@gmail.com">utkarshraj27122010@gmail.com</a></p>
            </div>
        </div>
    </body>
    </html>
    """

if __name__ == '__main__':
    app.run(debug=True)
