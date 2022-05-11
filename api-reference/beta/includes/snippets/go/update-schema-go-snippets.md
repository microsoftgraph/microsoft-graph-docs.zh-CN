---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89d28f862f6339377e13c3ce5093476f73883886
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326265"
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
externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Schema().Patch(requestBody)


```