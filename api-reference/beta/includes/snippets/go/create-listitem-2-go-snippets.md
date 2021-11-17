---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51b0dca1bd44d7e8ea807fba2cf0ced380e3edee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012023"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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