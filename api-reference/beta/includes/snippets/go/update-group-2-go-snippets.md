---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f81f030973bdd2e2a5edf7402a080bdd60e401a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411660"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
requestBody.SetAssignedLabels( []AssignedLabel {
    msgraphsdk.NewAssignedLabel(),
    SetAdditionalData(map[string]interface{}{
        "labelId": "45cd0c48-c540-4358-ad79-a3658cdc5b88",
    }
}
options := &msgraphsdk.GroupRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Patch(options)


```