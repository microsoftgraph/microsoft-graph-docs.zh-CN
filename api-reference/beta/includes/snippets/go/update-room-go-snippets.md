---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1df4574c31f4411d76430b9ae1f98d8efbe97f4d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011191"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlace()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.room",
    "nickname": "Conf Room",
    "building": "1",
    "label": "100",
    "capacity": ,
    "isWheelChairAccessible": false,
}
options := &msgraphsdk.PlaceRequestBuilderPatchOptions{
    Body: requestBody,
}
placeId := "place-id"
graphClient.PlacesById(&placeId).Patch(options)


```