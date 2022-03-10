---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d59ea4d001ff810ea7b3b76586525a17be2e2858
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412605"
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
options := &msgraphsdk.UpdateTiIndicatorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().UpdateTiIndicators().Post(options)


```