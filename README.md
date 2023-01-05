# gp-engine

Cosa para procesar un juego de gp ya que ya me jodería contar a mano todos estos gps de cada vez más jugadores.
El programa genera una tabla dónde por cada día aparece la hora del MBD, la hora en la que los jugadores han gepeado y, entre otras cosas, la hora del drg. También detecta las posibles faltas que han habido cada día (gps fuera del periodo legal para gepear).

La idea es que se revise la tabla y se decida qué faltas son legítimas y cuáles no. No se pretende procesar a la perfección el juego sino ayudar a hacerlo.

## Instrucciones
- Instalar dependencias: ```pandas```, ```numpy```, ```openpyxl```
```
$ pip install pandas
$ pip install numpy
$ pip install openpyxl
```
- Colocar el chat exportado del grupo en ```/chats/chat.txt```. (Debe ser renombrado a ```chat.txt```)
- Ejecutar ```main.py```
```
$ python main.py
```
- Si no hay errores, se creará el archivo ```out.csv```. Google Sheets lo abre perfectamente, en excel a veces faltan valores por alguna razón.

## Notas
Dependiendo de quién exporte el chat y cómo tenga agregadas en los contactos al resto de personas podrían aparecer errores que me da mucha pereza comprobar. De momento si el chat es exportado por Aitor o Anton debería funcionar. 
Si es necesario, se pueden añadir otros nombres diferentes en ```read_txt()``` dentro de ```gp.py```...




