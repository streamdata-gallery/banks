---
swagger: "2.0"
x-collection-name: Standard Chartered
x-complete: 0
info:
  title: Standard Chartered Bank Code Inquiry
  description: "The \u201CGetBankCode\u201D API returns list of Bank Codes for the
    specified combination of \u201CCountry\u201D, \u201CCity\u201D and \u201CBank\u201D
    combination. The data will contain the \u201CBank Code(s)\u201D as well as the
    address for the Bank & Branch."
  termsOfService: https://www.sc.com/terms-and-conditions
  contact:
    name: Steve Spicer
    url: https://www.sc.com
    email: steven.spicer@sc.com
  version: 1.0.0
host: developer.sc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cib/service/s2b/api/v1/banks/scb/accounts/{accountId}/{viewId}/account:
    get:
      summary: Accounts
      description: "The \u201CGetAccountBalance\u201D API upon successful user authentication
        and entitlement checks will return the various types of \u201CAccount Balances\u201D
        applicable for the specified Account Number."
      operationId: getCibServiceS2bApiV1BanksScbAccountsAccountViewAccount
      x-api-path-slug: cibservices2bapiv1banksscbaccountsaccountidviewidaccount-get
      parameters:
      - in: path
        name: accountId
      - in: header
        name: GroupId
      - in: header
        name: UserId
      - in: path
        name: viewId
      responses:
        200:
          description: OK
      tags:
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Banks
      - Scb
      - Accounts
      - Account
      - View
      - Account
  /cib/service/s2b/api/v1/banks/scb/accounts/{accountId}/{viewId}/transaction-request-types:
    get:
      summary: Finds all support transaction types for a given account
      description: "The \u201CGetTransactionTypes\u201D API upon successful user authentication
        and entitlement checks will return the supported transaction types for the
        specified account"
      operationId: getCibServiceS2bApiV1BanksScbAccountsAccountViewTransactionRequestTypes
      x-api-path-slug: cibservices2bapiv1banksscbaccountsaccountidviewidtransactionrequesttypes-get
      parameters:
      - in: path
        name: accountId
      - in: header
        name: GroupId
      - in: header
        name: UserId
      - in: path
        name: viewId
      responses:
        200:
          description: OK
      tags:
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Banks
      - Scb
      - Accounts
      - Account
      - View
      - Transaction
      - Request
      - Types
  /cib/service/s2b/api/v1/banks/scb/accounts/{viewId}/accounts:
    get:
      summary: Account Details & Balances
      description: List available bank accounts
      operationId: getCibServiceS2bApiV1BanksScbAccountsViewAccounts
      x-api-path-slug: cibservices2bapiv1banksscbaccountsviewidaccounts-get
      parameters:
      - in: header
        name: GroupId
      - in: header
        name: UserId
      - in: path
        name: viewId
      responses:
        200:
          description: OK
      tags:
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Banks
      - Scb
      - Accounts
      - View
      - Accounts
  /cib/service/s2b/api/v1/banks/scb/reference/default/branches:
    post:
      summary: Bank Code Inquiry
      description: "The \u201CGetBankCode\u201D API returns list of Bank Codes for
        the specified combination of \u201CCountry\u201D, \u201CCity\u201D and \u201CBank\u201D
        combination. The data will contain the \u201CBank Code(s)\u201D as well as
        the address for the Bank & Branch."
      operationId: postCibServiceS2bApiV1BanksScbReferenceDefaultBranches
      x-api-path-slug: cibservices2bapiv1banksscbreferencedefaultbranches-post
      responses:
        200:
          description: OK
      tags:
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Banks
      - Scb
      - Reference
      - Default
      - Branches
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---