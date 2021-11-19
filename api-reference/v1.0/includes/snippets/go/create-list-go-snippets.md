---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daeb0340166f1a8956e89c905f22f1058e61bfac
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099834"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewList()
displayName := "Books"
requestBody.SetDisplayName(&displayName)
requestBody.SetColumns( []ColumnDefinition {
    msgraphsdk.NewColumnDefinition(),
    SetAdditionalData(map[string]interface{}{
        "name": "Author",
    }
    msgraphsdk.NewColumnDefinition(),
    SetAdditionalData(map[string]interface{}{
        "name": "PageCount",
    }
}
list := msgraphsdk.NewListInfo()
requestBody.SetList(list)
template := "genericList"
list.SetTemplate(&template)
options := &msgraphsdk.ListsRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Lists().Post(options)


```