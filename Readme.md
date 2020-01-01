step 1. clone the repository 

         git clone https://github.com/hiteshpm/kyc.git

step2. setup network

        ##### Terminal Window 1

        run ./runApp.sh
* This launches the required network on your local machine
* Installs the fabric-client and fabric-ca-client node modules
* And, starts the node app on PORT 4000

Step 3. ##### Terminal Window 2

       In order for the following shell script to properly parse the JSON, you must install ``jq``:

instructions [https://stedolan.github.io/jq/](https://stedolan.github.io/jq/)

With the application started in terminal 1, next, test the APIs by executing the script - **testAPIs.sh**:

## To use golang chaincode execute the following command

./testAPIs.sh -l golang

 above script contain Rest api to register user, create channel, join channel, install chaincode, instantiate the chaincode and query kyc data.

 script contain below methods
 1. bulkupload : it  consumes "utildata.json" file (which contain some data)
                  and upload data in bulk.

2. QueryAllKyc:  IT will fetch all kyc data stored inside ledger
3. QueryKyc:   query single record.
4. requestLoan: it will create new loan request.

