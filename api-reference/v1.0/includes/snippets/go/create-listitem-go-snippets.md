---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c7b4afb003d92f9307be7ac2f20759e0df1d859
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewListItem()
fields := msgraphsdk.NewFieldValueSet()
requestBody.SetFields(fields)
fields.SetAdditionalData(map[string]interface{}{
    "Title": "Widget",
    "Color": "Purple",
    "Weight": ,
}
options := &msgraphsdk.ItemsRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).Items().Post(options)


```