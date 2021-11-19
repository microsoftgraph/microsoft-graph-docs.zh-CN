---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9215b16aec5a0bc2850aa595548a1212ab70f3f7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemAddress()
displayName := "Home"
requestBody.SetDisplayName(&displayName)
detail := msgraphsdk.NewPhysicalAddress()
requestBody.SetDetail(detail)
type := "home"
detail.SetType(&type)
detail.SetPostOfficeBox(nil)
street := "221B Baker Street"
detail.SetStreet(&street)
city := "London"
detail.SetCity(&city)
detail.SetState(nil)
countryOrRegion := "United Kingdom"
detail.SetCountryOrRegion(&countryOrRegion)
postalCode := "E14 3TD"
detail.SetPostalCode(&postalCode)
options := &msgraphsdk.AddressesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Addresses().Post(options)


```