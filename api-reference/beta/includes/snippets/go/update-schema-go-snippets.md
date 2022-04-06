---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8881edd8670947daa6ed599f3e5bc8b9b4b753f
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528199"
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
graphClient.External().ConnectionsById(&externalConnectionId).Schema().Patch(options)


```