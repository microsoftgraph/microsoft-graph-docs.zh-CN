---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9945add7e219c99d9a6cac6915c39e9e800a20ba
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328006"
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
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).Customers().Post(requestBody)


```