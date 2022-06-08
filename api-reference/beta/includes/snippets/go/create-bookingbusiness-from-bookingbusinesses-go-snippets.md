---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d97fc049de442d3fb59582728f075c17df9027c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946829"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingBusiness()
displayName := "Fourth Coffee"
requestBody.SetDisplayName(&displayName)
address := msgraphsdk.NewPhysicalAddress()
requestBody.SetAddress(address)
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
result, err := graphClient.BookingBusinesses().Post(requestBody)


```