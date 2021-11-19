---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2077b40a2b26c986240a2e0d74ec22b5f0fa67d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102131"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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