---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eac8a5a6c0f97003e8b7fb5811fee081a283603b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081988"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFieldValueSet()
requestBody.SetAdditionalData(map[string]interface{}{
    "Color": "Fuchsia",
    "Quantity": ,
}
options := &msgraphsdk.FieldsRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Fields().Patch(options)


```