## First
  - `cp .env.template .env`
  - You need to create the storage data path to do `docker-compose up`
    - `${VW_DATAPATH}` and `${DB_DATAPATH}`

## ADMIN_TOKEN
  - generate token
    `echo -n "MySecretPassword" | argon2 "$(openssl rand -base64 32)" -e -id -k 65540 -t 3 -p 4`

## login admin page
  - admin page url `https://yourdomain/admin`

## If you don't want to use SMTP server
  - You need to open the sign-up function on the admin page. After creating the accounts, you can then close it again.
