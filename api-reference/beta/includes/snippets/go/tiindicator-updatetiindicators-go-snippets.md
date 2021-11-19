---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ada810989b65ed71e925303a8459746ddd3df71
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084988"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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