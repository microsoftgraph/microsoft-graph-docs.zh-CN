---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade04687a39acc296180f16dcf4a8c08e20fd66a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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