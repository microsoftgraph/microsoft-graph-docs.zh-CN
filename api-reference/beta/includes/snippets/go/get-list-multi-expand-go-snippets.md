---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e89c9cc8a03276bb125b07b7ec98c0c964dcf83b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020747"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ListRequestBuilderGetQueryParameters{
    Select: "name,lastModifiedDateTime",
    Expand: "columns(select=name,description),items)",
}
options := &msgraphsdk.ListRequestBuilderGetOptions{
    Q: requestParameters,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).Get(options)


```