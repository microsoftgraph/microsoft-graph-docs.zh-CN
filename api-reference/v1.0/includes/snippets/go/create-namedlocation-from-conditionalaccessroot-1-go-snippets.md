---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b91466422008bbfde7c7be279e377564d34c08a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081895"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Untrusted IP named location"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "isTrusted": false,
    "ipRanges":  []Object {
    }
}
options := &msgraphsdk.NamedLocationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Post(options)


```