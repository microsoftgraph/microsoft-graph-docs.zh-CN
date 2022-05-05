---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f593714a4ea1d8f30be5eb11e94ffc52ae0868da
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211494"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDocumentSetVersion()
comment := "v1"
requestBody.SetComment(&comment)
shouldCaptureMinorVersion := false
requestBody.SetShouldCaptureMinorVersion(&shouldCaptureMinorVersion)
options := &msgraphsdk.DocumentSetVersionsRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).DocumentSetVersions().Post(options)


```