---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db6dd7c4273eb11fd567fc770ab3d93b800744ab
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412563"
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
result, err := graphClient.GroupsById(&groupId).Patch(options)


```