---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f85a25b8ebecf0b09c41028288fde8aefc3d8593
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412610"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
result, err := graphClient.PlacesById(&placeId).Patch(options)


```