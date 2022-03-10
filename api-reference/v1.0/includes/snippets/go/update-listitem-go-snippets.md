---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a393d36f433b064266fe2f009417c1a74ec24d22
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412199"
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
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Fields().Patch(options)


```