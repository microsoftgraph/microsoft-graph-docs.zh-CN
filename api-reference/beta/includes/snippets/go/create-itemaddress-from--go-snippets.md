---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ae1ab11c923c846a5ff0c9a4c7200eff0448183
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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