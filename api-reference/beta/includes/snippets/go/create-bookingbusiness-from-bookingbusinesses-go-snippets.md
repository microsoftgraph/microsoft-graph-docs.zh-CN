---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca61acc083f0b512789c9d512510a7af4e162cb4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328172"
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
result, err := graphClient.BookingBusinesses().Post(requestBody)


```