---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39c9ecfa0ac00980e8cc46f3d032232ab453bc01
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325851"
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
placeId := "place-id"
graphClient.PlacesById(&placeId).Patch(requestBody)


```