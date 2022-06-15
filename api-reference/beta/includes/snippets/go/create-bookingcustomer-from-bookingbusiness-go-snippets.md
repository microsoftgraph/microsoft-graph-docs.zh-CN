---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5edbd2a72b20a799c919bc8ab74d48e20188095
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098686"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomer()
displayName := "Joni Sherman"
requestBody.SetDisplayName(&displayName)
emailAddress := "jonis@relecloud.com"
requestBody.SetEmailAddress(&emailAddress)
requestBody.SetAddresses( []PhysicalAddress {
    msgraphsdk.NewPhysicalAddress(),
postOfficeBox := ""
    SetPostOfficeBox(&postOfficeBox)
street := "4567 Main Street"
    SetStreet(&street)
city := "Buffalo"
    SetCity(&city)
state := "NY"
    SetState(&state)
countryOrRegion := "USA"
    SetCountryOrRegion(&countryOrRegion)
postalCode := "98052"
    SetPostalCode(&postalCode)
type := "home"
    SetType(&type)
    msgraphsdk.NewPhysicalAddress(),
postOfficeBox := ""
    SetPostOfficeBox(&postOfficeBox)
street := "4570 Main Street"
    SetStreet(&street)
city := "Buffalo"
    SetCity(&city)
state := "NY"
    SetState(&state)
countryOrRegion := "USA"
    SetCountryOrRegion(&countryOrRegion)
postalCode := "98054"
    SetPostalCode(&postalCode)
type := "business"
    SetType(&type)
}
requestBody.SetPhones( []Phone {
    msgraphsdk.NewPhone(),
number := "206-555-0100"
    SetNumber(&number)
type := "home"
    SetType(&type)
    msgraphsdk.NewPhone(),
number := "206-555-0200"
    SetNumber(&number)
type := "business"
    SetType(&type)
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).Customers().Post(requestBody)


```