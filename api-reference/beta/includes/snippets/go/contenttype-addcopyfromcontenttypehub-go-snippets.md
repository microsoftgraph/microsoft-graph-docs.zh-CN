---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb401bd8df28d56c349cd6dd9ece77fd01bae6a3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411770"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentTypeIdRequestBody()
contentTypeId := "String"
requestBody.SetContentTypeId(&contentTypeId)
options := &msgraphsdk.AddCopyFromContentTypeHubRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopyFromContentTypeHub(site-id, list-id).Post(options)


```