# learn-voxology
This project was created to assist me in learning voxology API.

## Tutorials: 

http://voxolo.gy/service/programmable-voice/#getting-started

----

#NOTES

## Receive Calls

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

5. Call the phone number

## Make Calls

1. Find and provision a number using voxology API (See steps 1,2 of *Receive Calls Steps* section)

2. Call the endpoint
`POST Dials/Connect`

## Multi-Action Processing

1. See `goto.json` file 

## Conditional Processing

1. See `if.json` file 


