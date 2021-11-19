---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f326114d8b25a060e97ce660153e1d2252eee7fe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089607"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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