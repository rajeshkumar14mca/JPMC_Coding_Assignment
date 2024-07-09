# JPMC_Coding_Assignment

Seven Service created for this project
1. Service-Registry
2. Api-gateway
3. accounts-service
4. positions-service
5. eligibility-service
6. price-service
7. fx-service

Develop a service which calculates collateral value & market value for given accounts, which hold certains positions.
Position = units (quantity) of certain assets, identified by assetId
Collateral value for account = Sum of collateral value for all positions in a given account.
Collateral value for ‘eligible’ position = quantity x price x discount factor
Collateral value for ‘ineligible’ position = Zero
Market value for both ‘eligible’ & ‘ineligible’ positions = quantity x price

Having some doubt in Market value, I assumed market value also Sum of all positions in a given account.
Having doubt in calculation for Collateral value and Market value. Did all the calulation using USD and finaly convert into given currency

Path
===========
http://localhost:8051/accounts/accountsList

Body
==============
{
    "accountsId":["E1"],
    "currencyCode":"GBP"
}

