# learn-voxology
This project was created to assist me in learning voxology API

## Steps:
1. Search numbers
`GET /PhoneNumbers/Available`

2. Once found numbers you need to provision them
`POST PhoneNumbers/CallFlows`

3. Configure your callback and uploaded to some
file server.
`See hello-worl.json file`

4. Let voxology know about your callback
`PUT CallFlows/Configurations/PhoneNumbers/[PHONE_NUMBER]`

PHONE_NUMBER format is +13239029991, but you need to
URL encode it into %2B13239029991 (+ -> %2B)
