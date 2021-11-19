---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6e3ac3c3e295f29dc06927813f593ea50d635f9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084598"
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
graphClient.GroupsById(&groupId).Patch(options)


```