#flask
from flask import Flask, url_for, request, render_template;
from app import app



#Server/
@app.route('/', methods=['POST','GET'])
def home():
    return render_template('paginaincio.html')
    if request.method == 'POST':
        #esto leera la info de la persona y guardara para buscarla
        titulo = request.form['titulo']
        fecha = request.form['fecha']
        autor = request.form['autor']
        #regresar la informacion encontrada
        return render_template('paginarespuesta.html', titulo=titulo, fecha=fecha, autor=autor );
    else:
        return render_template('Eror404.html')

