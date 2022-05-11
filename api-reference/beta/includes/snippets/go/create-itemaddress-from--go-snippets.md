---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 991765257460a8c9e3d62d4bef1142c584fc6853
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328839"
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
result, err := graphClient.Me().Profile().Addresses().Post(requestBody)


```