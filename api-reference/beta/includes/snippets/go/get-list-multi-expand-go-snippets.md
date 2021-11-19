---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 843525ed695bdc1202648efa6f52fc49c3f235ee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096310"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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