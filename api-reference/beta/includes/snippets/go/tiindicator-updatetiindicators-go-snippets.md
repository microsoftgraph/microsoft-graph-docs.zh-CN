---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e143f33ddbf1d065dae9daf583934cc081b025df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989433"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetValue( []TiIndicator {
    msgraphsdk.NewTiIndicator(),
    SetAdditionalData(map[string]interface{}{
        "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
        "additionalInformation": "mytest",
    }
    msgraphsdk.NewTiIndicator(),
    SetAdditionalData(map[string]interface{}{
        "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
        "additionalInformation": "test again",
    }
}
options := &msgraphsdk.UpdateTiIndicatorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().UpdateTiIndicators().Post(options)


```