---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4806a77aa04028997d3e83650004cba5ae4776b6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974214"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
contentType := "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101"
requestBody.SetContentType(&contentType)
options := &msgraphsdk.AddCopyRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopy().Post(options)


```