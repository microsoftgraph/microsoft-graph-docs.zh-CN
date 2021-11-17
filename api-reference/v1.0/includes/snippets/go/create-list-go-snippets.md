---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fcabf06ab3c57de93bff6bc5a8ab9b4bff8f29a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023412"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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