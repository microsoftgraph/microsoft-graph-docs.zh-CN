---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4636de8b4287e64cde6316cd508fc1e077bc930e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090620"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingBusiness()
displayName := "Fourth Coffee"
requestBody.SetDisplayName(&displayName)
address := msgraphsdk.NewPhysicalAddress()
requestBody.SetAddress(address)
type := "mall"
address.SetType(&type)
postOfficeBox := "P.O. Box 123"
address.SetPostOfficeBox(&postOfficeBox)
street := "4567 Main Street"
address.SetStreet(&street)
city := "Buffalo"
address.SetCity(&city)
state := "NY"
address.SetState(&state)
countryOrRegion := "USA"
address.SetCountryOrRegion(&countryOrRegion)
postalCode := "98052"
address.SetPostalCode(&postalCode)
phone := "206-555-0100"
requestBody.SetPhone(&phone)
email := "manager@fourthcoffee.com"
requestBody.SetEmail(&email)
webSiteUrl := "https://www.fourthcoffee.com"
requestBody.SetWebSiteUrl(&webSiteUrl)
defaultCurrencyIso := "USD"
requestBody.SetDefaultCurrencyIso(&defaultCurrencyIso)
options := &msgraphsdk.BookingBusinessesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.BookingBusinesses().Post(options)


```