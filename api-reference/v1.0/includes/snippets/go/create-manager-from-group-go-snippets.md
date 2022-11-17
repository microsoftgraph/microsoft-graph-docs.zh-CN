---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 625643bea739de0b09780ca938ccfe5d560dfd38
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992310"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}",
}
options := &msgraphsdk.RefRequestBuilderPutOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Manager().$ref().Put(options)


```