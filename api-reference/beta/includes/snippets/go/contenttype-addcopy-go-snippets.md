---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2fd5c0d0040564de50ebb93462bb010cd9c979d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
contentType := "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
requestBody.SetContentType(&contentType)
options := &msgraphsdk.AddCopyRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopy().Post(options)


```