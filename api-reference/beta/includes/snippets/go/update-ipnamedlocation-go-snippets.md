---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4704f7c5b8854c71e5a5e4596f4b3fcc8c96c878
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094294"
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
graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Patch(options)


```