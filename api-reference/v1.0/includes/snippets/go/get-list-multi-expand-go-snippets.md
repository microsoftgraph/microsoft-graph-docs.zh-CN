---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c043fcb487d66d991cdc44d111b29adc13216c39
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ListRequestBuilderGetQueryParameters{
    Select: "id,name,lastModifiedDateTime",
    Expand: "columns(select=name,description),items)",
}
options := &msgraphsdk.ListRequestBuilderGetOptions{
    Q: requestParameters,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).Get(options)


```