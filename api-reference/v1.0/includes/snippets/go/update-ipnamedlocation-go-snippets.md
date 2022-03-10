---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c419714510c54c2bb3c4e7a48a97032f9003d793
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412201"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Untrusted named location with only IPv4 address"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "isTrusted": false,
    "ipRanges":  []Object {
    }
}
options := &msgraphsdk.NamedLocationRequestBuilderPatchOptions{
    Body: requestBody,
}
namedLocationId := "namedLocation-id"
result, err := graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Patch(options)


```