--Explicación para ejecutar este sistema--
1.- Primero tenemos que clonar el repositorio en la terminal (CTRL + Ñ) usando:
´´git clone https://github.com/FcoINF/EVA1_IA.git

2.- y ahora hay que entrar al terminal git bash y revisar si estamos dentro de nuestro directorio, si no lo esta entonces hay que ejecutar lo siguiente:
´´cd EVA1_IA

Es necesario instalar lo siguiente:
´´pip install -r requirements.txt
´´pip install openai

3.- Una vez listo, en las variables base_url ingresamos la URL de GitHub base ("https://models.inference.ai.azure.com")
y en api_key ingresamos nuestro token de GitHub, y se podra ejecutar el codigo completo (revisar si nuestros tokens están expirados o no, si lo están, hay que crear nuevos).

4.- Luego tendremos que exportar estas variables usando export, asi como se muestra abajo:
´´export base_url="GITHUB_BASE_URL"
´´api_key="GITHUB_TOKEN"

5.- Y finalmente entrar a jupyter lab, para esto hay que escribir en el terminal git bash:
´´jupyter lab
Si no esta instalado hay que ejecutar lo siguiente:
´´pip install jupyter lab
Finalmente se abrira una ventana en la que tenemos que elegir el ipykernel, se tendra que seleccionar el de Notebook python3 (ipyKernel) .

--Explicacion del funcionamiento del codigo--
Dentro de nuestro menú están las opciones que se pueden elegir para preguntar dentro del sitio web,
hay 4 opciones y cada una le da el contexto a la IA sobre lo que el usuario le va a preguntar, 
menos la de chat general que es una conversación directa con la IA, y con una opción para salir.

Las opciones se eligen mediante un numero del 1 al 6 que elija el usuario, dependiendo de la opción,
se informa a la IA el tema sobre lo que el usuario esta preguntando, si la opción ingresada no es un
numero entero o es una opción que no existe, avisara al usuario que es una opción inválida.

ahora mismo se añadió 3 opciones para la respuesta de la IA, esta Zero-shot, Few-shot y Chain of Thought, el usuario podrá elegir una de estas tres tipos de respuestas en la que cada una tiene distintas formas de explicarlo.

--Problemática--

La problematica a solucionar en base a este proyecto es facilitar a los usuarios realizar consultas o tener un acesso
directo a lo que buscan apenas entrar a la página de la municipalidad, en base a esto podemos optimizar muchos procesos gracias al
ChatBOT.
