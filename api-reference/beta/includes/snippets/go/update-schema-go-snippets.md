---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbd529d696dc1e0859abb2f298ae963bc779c43e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395466"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSchema()
baseType := "microsoft.graph.externalItem"
requestBody.SetBaseType(&baseType)
requestBody.SetProperties( []Property {
    msgraphsdk.NewProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "ticketTitle",
        "type": "string",
        "isSearchable": "true",
        "isRetrievable": "true",
        "labels":  []String {
            "title",
        }
    }
    msgraphsdk.NewProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "priority",
        "type": "string",
        "isQueryable": "true",
        "isRetrievable": "true",
        "isSearchable": "false",
    }
    msgraphsdk.NewProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "assignee",
        "type": "string",
        "isRetrievable": "true",
    }
}
options := &msgraphsdk.SchemaRequestBuilderPatchOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).Schema().Patch(options)


```