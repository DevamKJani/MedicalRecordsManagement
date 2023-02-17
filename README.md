# Medical Records Management System

Healthcare Management, moved over Blockchain!

## Developers
The project is developed by
- Harsh Keshruwala
- Devam Kalpesh Jani

# Instructions to run the API Backend
- clone the repo - https://github.com/DevamKJani/MedicalRecordsManagement.git
- move to the directory we cloned in the previous step `cd HM_System`.
- At first, install [Hyperledger composer](https://hyperledger.github.io/composer/latest/installing/installing-prereqs.html). Then install the [development environment](https://hyperledger.github.io/composer/latest/installing/development-tools.html).
- In order to setup your Blockchain network and generate Hyperledger Composer Rest Server, execute the following commands:
- `composer archive create -t dir -n .`
- `composer network install --card PeerAdmin@hlfv1 --archiveFile ehr@0.0.3.bna`
- `composer network start --networkName ehr --networkVersion 0.0.3 --card PeerAdmin@hlfv1 --networkAdmin admin --networkAdminEnrollSecret adminpw --file networkadmin.card`
- `composer card import --file networkadmin.card` 
- `composer-rest-server -c admin@ehr -n always -u true -d y -w true`
- Go to `http://localhost:3000/explorer` to explore the REST API server


# Instructions to restart the REST API
- change the directory to "/fabric-dev-servers/fabric-scripts/hlfv1/composer" to access the docker-compose.yml file
- Run `docker-compose stop` to stop the Fabric Containers.
- Run `docker-compose start` to restart from where you left off.
- get into the cloned repository's directory: cd /fabric-dev-servers/MedicalRecordsManagement
- Run this command to start the server: `composer-rest-server -c admin@medicalrecords -n always -u true -d y -w true`
- Go to `http://localhost:3000/explorer` to explore the REST API.


# Output
![1](https://user-images.githubusercontent.com/81607787/114814939-dd836180-9dd2-11eb-8609-257089091265.png)
![2](https://user-images.githubusercontent.com/81607787/114814941-df4d2500-9dd2-11eb-9357-b209a63d864b.png)
![3](https://user-images.githubusercontent.com/81607787/114814944-e07e5200-9dd2-11eb-805b-d5612e0a71e5.png)
![4](https://user-images.githubusercontent.com/81607787/114814948-e1af7f00-9dd2-11eb-8b24-1a6154a1282c.png)
![5](https://user-images.githubusercontent.com/81607787/114814954-e2e0ac00-9dd2-11eb-920f-6d8ddfcd1fdf.png)
![6](https://user-images.githubusercontent.com/81607787/114814960-e5430600-9dd2-11eb-84a5-3ec2f3ebc368.png)
![7](https://user-images.githubusercontent.com/81607787/114814966-e70cc980-9dd2-11eb-91c7-2cac867659b2.png)
![8](https://user-images.githubusercontent.com/81607787/114814969-e83df680-9dd2-11eb-949f-6fdba6498b74.png)
![9](https://user-images.githubusercontent.com/81607787/114814970-e96f2380-9dd2-11eb-9ab2-48ff111faeda.png)
![10](https://user-images.githubusercontent.com/81607787/114814973-ea07ba00-9dd2-11eb-8148-beffa2a56ec4.png)
![12](https://user-images.githubusercontent.com/81607787/114814976-eb38e700-9dd2-11eb-8a17-406c7096f2f4.png)
![13](https://user-images.githubusercontent.com/81607787/114814979-ec6a1400-9dd2-11eb-8ba2-989f1cce714d.png)
![14](https://user-images.githubusercontent.com/81607787/114814984-ed9b4100-9dd2-11eb-95b4-7979a13e5962.png)
