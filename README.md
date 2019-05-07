# ![LOGO](logo.png) Just Eat Tenant API **flow**ground Connector

## Description

A generated **flow**ground connector for the Just Eat Tenant API API (version 2.0.0.0).

Generated from: https://api.apis.guru/v2/specs/je-apis.com/2.0.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:32+03:00

## API Description



## Authorization

This API does not require authorization.

## Actions

### Gets the status

> Uri template /application/onlinestatus

*Tags:* `application`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Gets the application version and status

> Uri template /application/{applicationId}/versionstatus/{versionId}

*Tags:* `application`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `applicationId` - _required_
* `versionId` - _required_

### Gets the application version [Obsolete (As verified by Android/Ios on 23-02-2016)]

> Uri template /application/{applicationId}/versionupdate/{versionId}

*Tags:* `application`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `applicationId` - _required_
* `versionId` - _required_

### Creates a Basket

> Uri template /baskets

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Gets a Basket

> Uri template /baskets/{basketId}

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Set order contact details

> Uri template /baskets/{basketId}/contactdetails/

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Set preferred order fulfilment time. We're expecting the time to be one of the choices that you got back from the GET, unadjusted for timezone.

> Uri template /baskets/{basketId}/fulfilmenttime?time={time}&asap={asap}

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_
* `time` - _optional_
* `asap` - _optional_

### Get available fulfilment times for basket

> Uri template /baskets/{basketId}/fulfilmenttimeslots/

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### ***STUB*** Set order notes

> Uri template /baskets/{basketId}/notes

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Add products into a given basket

> Uri template /baskets/{basketId}/orderitems

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Remove products from a given basket

> Uri template /baskets/{basketId}/orderitems/{orderItemId}

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_
* `orderItemId` - _required_

### Add meal parts into a given product inside a given basket

> Uri template /baskets/{basketId}/orderitems/{orderItemId}/mealparts

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_
* `orderItemId` - _required_

### Add optional accessories into a given product inside a given basket

> Uri template /baskets/{basketId}/orderitems/{orderItemId}/optionalaccessories

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_
* `orderItemId` - _required_

### Add required accessories into a given product inside a given basket

> Uri template /baskets/{basketId}/orderitems/{orderItemId}/requiredaccessories

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_
* `orderItemId` - _required_

### Get payment options for a basket

> Uri template /baskets/{basketId}/paymentoptions?applePay={applePay}&androidPay={androidPay}&googlePay={googlePay}&platform={platform}&voucherCode={voucherCode}

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_
* `platform` - _optional_
* `applePay` - _optional_
* `androidPay` - _optional_
* `googlePay` - _optional_
* `voucherCode` - _optional_
* `Auth-Token` - _optional_

### Change service options for Basket

> Uri template /baskets/{basketId}/serviceoptions

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Updates a user of a basket

> Uri template /baskets/{basketId}/user

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Update zipcode from a given basket

> Uri template /baskets/{basketId}/zipcode

*Tags:* `baskets`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Gets a consumer via either Basic Authorization/Auth-Token or a Bearer token

> Uri template /consumer

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Updates a consumer

> Uri template /consumer

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Creates a consumer

> Uri template /consumer

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Gets a consumers addresses by the Auth-Token header

> Uri template /consumer/addresses

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Delete a device token for a consumer

> Uri template /consumer/devicetokens

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Activate a device token for a consumer

> Uri template /consumer/devicetokens

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Returns statuses for InFlight orders for a given consumer

> Uri template /consumer/inflight-order-status<br/><br/>Accept-Version:1 StatusNames: <br/>['AwaitingPayment' or 'Processing' or 'Completed' or 'Canceled' or 'Declined' or 'Accepted' or 'OnItsWay' or 'DueDateChanged']<br/><br/>Accept-Version:2 StatusNames: <br/>['DueDateDelayed']<br/><br/>Accept-Version:3 StatusNames: <br/>['OrderReady']<br/><br/>Accept-Version:4 StatusNames: <br/>['PreOrderPending']

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_
* `Accept-Version` - _required_

### Return order history by Auth-Token

> Uri template /consumer/order-history?page={page}&pageSize={pageSize}

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `page` - _optional_
* `pageSize` - _optional_
* `Auth-Token` - _optional_

### Changes a consumer password and logs in

> Uri template /consumer/password

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Get a consumers preferences by the Auth-Token header

> Uri template /consumer/preferences

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Update a consumers preferences by the Auth-Token header

> Uri template /consumer/preferences

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Returns the consumers serviceable addresses based the Auth-Token and the TR id

> Uri template /consumer/serviceable-addresses/restaurant/{restaurantId}

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_
* `maxAmount` - _optional_
* `Auth-Token` - _optional_

### Returns the consumers serviceable addresses based the Auth-Token and the TR id

> Uri template /consumer/serviceable-addresses/restaurant/{restaurantId}/{maxAmount}

*Tags:* `consumer`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_
* `maxAmount` - _required_
* `Auth-Token` - _optional_

### Get customisation info for Consumer Help

> Uri template /consumerhelp/customisation?orderid={orderid}&requestcontext={requestcontext}

*Tags:* `consumerhelp`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _optional_
* `requestContext` - _optional_

### Get the next flow step in a Consumer Help flow

> Uri template /consumerhelp/flows/{flow}/{orderId}/{action}

*Tags:* `consumerhelp`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `flow` - _required_
* `orderId` - _required_
* `action` - _required_

### Post to a Consumer Help flow and get the next step

> Uri template /consumerhelp/flows/{flow}/{orderId}/{action}

*Tags:* `consumerhelp`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `flow` - _required_
* `orderId` - _required_
* `action` - _required_

### Get the next flow step in a Consumer Help flow; extra URL segment

> Uri template /consumerhelp/flows/{flow}/{orderId}/{action}/{subaction}

*Tags:* `consumerhelp`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `flow` - _required_
* `orderId` - _required_
* `action` - _required_
* `subaction` - _required_

### Post to a Consumer Help flow and get the next step; extra URL segment

> Uri template /consumerhelp/flows/{flow}/{orderId}/{action}/{subaction}

*Tags:* `consumerhelp`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `flow` - _required_
* `orderId` - _required_
* `action` - _required_
* `subaction` - _required_

### Get all country codes - response is an array of strings

> Uri template /countries

*Tags:* `countries`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Get active experiments

> Uri template /experiments/active

*Tags:* `experiments`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### HealthHandler.Check

> Uri template /health/check

*Tags:* `health`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### HealthHandler.Check

> Uri template /health/validate

*Tags:* `health`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Testing validation

> Uri template /internal/for-testing/{basketId}/contactdetails/

*Tags:* `internal`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `basketId` - _required_

### Runs all known health checks - response is array of HealthCheckResult

> Uri template /internal/health/all

*Tags:* `internal`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Login a user and return an Auth-Token

> Uri template /logins

*Tags:* `logins`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Gets delivery areas from a given menu

> Uri template /menus/{menuId}/deliveryareas

*Tags:* `menus`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `menuId` - _required_

### Gets categories for a given menu

> Uri template /menus/{menuId}/productcategories

*Tags:* `menus`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `menuId` - _required_

### Gets all products from a given category

> Uri template /menus/{menuId}/productcategories/{categoryId}/products

*Tags:* `menus`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `menuId` - _required_
* `categoryId` - _required_

### Create an Order from a Basket

> SuccessState values are: Unknown = 0, Successful, InvalidBasket, BasketNotOrderable, PotentialDuplicate, BasketDoesNotExist, BasketTooBig, InvalidContactDetails, GuestAccountCannotBeCreated, InvalidAuthToken

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Gets an order by OrderId

> Uri template /orders/{orderId}

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Get campaign content details of orders that have been given away

> Uri template /orders/{orderId}/campaigncontent

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_

### Pay for an order using account credit

> Uri template /orders/{orderId}/pay/accountcredit

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Pay using Android Pay

> Uri template /orders/{orderId}/pay/android/

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Pay using Apple Pay

> Uri template /orders/{orderId}/pay/apple/

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Pay for an order using cash

> Uri template /orders/{orderId}/pay/cash

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Pay using Google Pay

> Uri template /orders/{orderId}/pay/google/

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Pay for an order using a saved card

> Uri template /orders/{orderId}/pay/savedcard

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Gets the current status of the payment for an order

> Uri template /orders/{orderId}/payment/status/

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_

### Get payment options for an order

> Uri template /orders/{orderId}/paymentoptions?applePay={applePay}&androidPay={androidPay}&googlePay={googlePay}&platform={platform}&voucherCode={voucherCode}

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `platform` - _optional_
* `applePay` - _optional_
* `androidPay` - _optional_
* `googlePay` - _optional_
* `voucherCode` - _optional_
* `Auth-Token` - _optional_

### Creates a new basket from a previous order

> Uri template /orders/{orderId}/reorder

*Tags:* `orders`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `orderId` - _required_
* `Auth-Token` - _optional_

### Submits a user review for a given order

> Uri template /ratings

*Tags:* `ratings`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `Auth-Token` - _optional_

### Creates a reset password token, initiates sending an email to the consumer with a link to reset their password. Device type will currently allow for customisation of email links; include if the calling device requires custom templates.

> Uri template /reset-password-tokens

*Tags:* `reset-password-tokens`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Search restaurants by free text

> Uri template /restaurants?freetext={freeText}&cuisine={cuisine}&name={restaurantName}

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `freeText` - _optional_
* `cuisine` - _optional_
* `restaurantName` - _optional_

### Gets available badges

> Uri template restaurants/available_badges

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Search V3 restaurants by postcode and/or cuisine type, version header kept for backwards compatibility

> Uri template /restaurants/v3?q={postCode}&c={cuisine}&name={restaurantName}

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `postCode` - _optional_
* `cuisine` - _optional_
* `restaurantName` - _optional_
* `Accept-Version` - _required_
* `UseSearchOrchestrator` - _optional_

### Gets restaurant details

> Uri template /restaurants/{restaurantId}/details

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_

### Gets menus of a restaurant

> Uri template /restaurants/{restaurantId}/menus?delivery={delivery}&current={current}&postcode={postcode}

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_
* `current` - _optional_
* `delivery` - _optional_
* `postcode` - _optional_

### Gets all available menus for a given restaurant and time

> Uri template /restaurants/{restaurantId}/menus/available?time={utcTime}

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_
* `utcTime` - _optional_

### Gets all product categories for a given restaurant

> Uri template /restaurants/{restaurantId}/productcategories?type={serviceType}&time={utcTime}&zipcode={zipcode}

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_
* `serviceType` - _optional_
* `utcTime` - _optional_
* `zipcode` - _optional_
* `Accept-Version` - _required_

### Get paged list of reviews for a given restaurant

> Uri template /restaurants/{restaurantId}/reviews?p={pageNumber}&s={pageSize}

*Tags:* `restaurants`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `restaurantId` - _required_
* `pageNumber` - _optional_
* `pageSize` - _optional_

### Gets the latest terms and conditions

> Uri template /terms

*Tags:* `terms`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_

### Gets zipcode autocomplete suggestions

> Uri template /zipcodeautocomplete?term={term}&resultsCount={resultsCount}

*Tags:* `zipcodeautocomplete`

#### Input Parameters
* `Accept-Tenant` - _required_ - uk
* `Authorization` - _required_
* `term` - _optional_
* `resultsCount` - _optional_

## License

**flow**ground :- Telekom iPaaS / je-apis-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
