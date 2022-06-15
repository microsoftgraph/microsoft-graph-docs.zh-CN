---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9badacf2303b13bd93de05ea84f782b9c687e4b9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSchema()
baseType := "microsoft.graph.externalItem"
requestBody.SetBaseType(&baseType)
requestBody.SetProperties( []Property {
    msgraphsdk.NewProperty(),
name := "ticketTitle"
    SetName(&name)
type := "string"
    SetType(&type)
isSearchable := "true"
    SetIsSearchable(&isSearchable)
isRetrievable := "true"
    SetIsRetrievable(&isRetrievable)
    SetLabels( []Label {
        "title",
    }
    msgraphsdk.NewProperty(),
name := "priority"
    SetName(&name)
type := "string"
    SetType(&type)
isQueryable := "true"
    SetIsQueryable(&isQueryable)
isRetrievable := "true"
    SetIsRetrievable(&isRetrievable)
isSearchable := "false"
    SetIsSearchable(&isSearchable)
    msgraphsdk.NewProperty(),
name := "assignee"
    SetName(&name)
type := "string"
    SetType(&type)
isRetrievable := "true"
    SetIsRetrievable(&isRetrievable)
}
externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Schema().Patch(requestBody)


```