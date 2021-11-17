---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bf78ca0a0f4d65a2de42e6646e429ba2f0df787
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029195"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.TeamRequestBuilderPutOptions{
    Body: requestBody,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Team().Put(options)


```