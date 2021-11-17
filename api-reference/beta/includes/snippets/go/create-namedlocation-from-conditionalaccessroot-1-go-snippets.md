---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d35b22803100550ed2d8e8c3d88a3356cca9e3a0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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