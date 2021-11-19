---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a91f21166281580938bd4396ac5ab1578cf9b424
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100756"
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
    SetAdditionalData(map[string]interface{}{
        "postOfficeBox": "",
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "countryOrRegion": "USA",
        "postalCode": "98052",
        "type": "home",
    }
    msgraphsdk.NewPhysicalAddress(),
    SetAdditionalData(map[string]interface{}{
        "postOfficeBox": "",
        "street": "4570 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "countryOrRegion": "USA",
        "postalCode": "98054",
        "type": "business",
    }
}
requestBody.SetPhones( []Phone {
    msgraphsdk.NewPhone(),
    SetAdditionalData(map[string]interface{}{
        "number": "206-555-0100",
        "type": "home",
    }
    msgraphsdk.NewPhone(),
    SetAdditionalData(map[string]interface{}{
        "number": "206-555-0200",
        "type": "business",
    }
}
options := &msgraphsdk.CustomersRequestBuilderPostOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).Customers().Post(options)


```