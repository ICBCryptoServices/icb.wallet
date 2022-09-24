

# ![alt text](https://github.com/ICBCryptoServices/icb.wallet/blob/main/ICB-Logo.png?raw=true) icb.wallet
This is distribute service ICB Wallet that user can deploy own ICB wallet on to own server


## System Requirements
  - [Install Git] (https://git-scm.com/downloads)
  - [Install Docker] (https://docs.docker.com/get-docker/)
  - [Install Docker Compose] (https://docs.docker.com/compose/install/)
  
  
## Get started
  ```ruby
git clone https://github.com/icbchain/icb.wallet.git
```
  

### Edit config env.config
  ```
export SERVER_NAME=[YOUR DOMAIN NAME]
```
> Note: [YOUR DOMAIN NAME] is domain address that you are registered for website!

## Configure SSL Certificates
### Edit SSL Key ssl.key in nginx/ssl/
  ```
-----BEGIN PRIVATE KEY-----
[YOUR PRIVATE KEY] 
-----END PRIVATE KEY-----
```
> Note: [YOUR PRIVATE KEY] is your ssl private key

### Edit SSL Cert ssl.crt in nginx/ssl/
  ```
-----BEGIN CERTIFICATE REQUEST-----
[YOUR CERTIFICATE REQUEST]
-----END CERTIFICATE REQUEST-----
-----BEGIN CERTIFICATE-----
[YOUR CERTIFICATE]
-----END CERTIFICATE-----
```
> Note: [YOUR CERTIFICATE REQUEST] is your ssl certificate request and [YOUR CERTIFICATE] is your ssl certificate



### Run a web wallet
open terminal and used command line
  ```ruby
$ cd icb.wallet
$ ./manage.sh init
$ ./manage.sh start
```


<details><summary>Important for Linux - Access Permission</summary>
<p>

> Note: ** if you are using linux you should access to manage.ssh **

```
$ chmod u=rwx,g=r,o=r manage.sh
```

</p>
</details>
