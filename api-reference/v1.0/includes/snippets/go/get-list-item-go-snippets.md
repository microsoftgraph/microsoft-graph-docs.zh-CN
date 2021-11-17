---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1d8892e459509e295d30be040c6b4078e8243cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ListItemRequestBuilderGetQueryParameters{
    Expand: "fields",
}
options := &msgraphsdk.ListItemRequestBuilderGetOptions{
    Q: requestParameters,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Get(options)


```