---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 701f284e399ae631fe493eb093aa8b8c7fb9713a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "baseType": "microsoft.graph.externalItem",
    "properties":  []Object {
    }
}
options := &msgraphsdk.SchemaRequestBuilderPostOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Schema().Post(options)


```