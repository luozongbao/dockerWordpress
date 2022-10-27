# dockerWordpress
1. download wordpress
```
wget https://wordpress.org/latest.zip
```
2. unzip
```
unzip latest.zip
```
3. Since we are using alpine image which have user/group www-data map at ID:82 then we should specify chown of wordpress to 82:82
```
chown -R 82:82 wordpress
```
4. spin it up!!
