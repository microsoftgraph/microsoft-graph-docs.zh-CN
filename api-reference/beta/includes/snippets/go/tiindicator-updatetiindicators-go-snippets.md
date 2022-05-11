---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a20d9840445bed48a72d62264591afec667c322b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329245"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewValueRequestBody()
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
result, err := graphClient.Security().TiIndicators().UpdateTiIndicators().Post(requestBody)


```