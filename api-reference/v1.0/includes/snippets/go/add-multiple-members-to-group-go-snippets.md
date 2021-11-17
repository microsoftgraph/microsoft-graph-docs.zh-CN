---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ec9a294798288aaedf6bf894a85ec3ba3d4ad75
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025296"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGroup()
requestBody.SetAdditionalData(map[string]interface{}{
    "members@odata.bind":  []String {
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    }
}
options := &msgraphsdk.GroupRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(options)


```