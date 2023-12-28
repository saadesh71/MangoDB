# MongoDB

### Install MongoDB (Self Note, not for students):
wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | sudo apt-key add -  
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list  
sudo apt-get update  
sudo apt-get install -y mongodb-org  
sudo systemctl start mongod   

If you receive an error similar to the following when starting mongod failed to start mongod.service: Unit mongod.service not found.  

Run the following command first:  
sudo systemctl daemon-reload  

* check if service is running:  
sudo systemctl status mongod  

* Stop MongoDB:  
sudo systemctl stop mongod  

* Restart MongoDB:  
sudo systemctl restart mongod  

* Begin using MongoDB:  
mongosh

# Question
![HW_MongoDB_2023](https://github.com/saadesh71/MongoDB/assets/43541169/0ca131f8-2176-47f1-a0d1-94fdd1d08352)

Dataset: [reviews_Books_5.json.gz](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Books_5.json.gz)
