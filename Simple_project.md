Simple project

SQLite3 configuration on RaspberryPi

Install sqlite3

`sudo apt install sqlite3`

Create database

`sqlite3 heart_attack.db`

Database will be created and sqlite opened as on the screenshot:

![image](https://github.com/user-attachments/assets/97d54119-26c6-4d16-bb92-911e2f8ed0dc)


Create table in database and import data from CSV
```
sqlite3 heart_attack.db <<EOF
.mode csv
.import heart_attack_young_adult_france.csv heart_attack_france
EOF
```

