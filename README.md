# How to install mongodb in ubuntu
1. referece: https://www.mongodb.com/docs/mongodb-shell/install/?linux-distribution=ubuntu&operating-system=linux&ubuntu-version=noble
2. run bellow command
```
 atulkrishnathakur@atul-pc:~$ wget -qO- https://www.mongodb.org/static/pgp/server-8.0.asc | sudo tee /etc/apt/trusted.gpg.d/server-8.0.asc
```

```
atulkrishnathakur@atul-pc:~$ sudo apt-get install gnupg

```

```
atulkrishnathakur@atul-pc:~$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu noble/mongodb-org/8.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-8.0.list

```

```
atulkrishnathakur@atul-pc:~$ sudo apt-get install -y mongodb-mongosh

```

```
atulkrishnathakur@atul-pc:~$ sudo apt install -y mongodb-org

```

```
atulkrishnathakur@atul-pc:~$ sudo systemctl enable mongod

```

```
atulkrishnathakur@atul-pc:~$ sudo systemctl start mongod

```

```
atulkrishnathakur@atul-pc:~$ sudo systemctl status mongod

```
3. run `mongosh` command and check 
