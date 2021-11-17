---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f06b1b98f5dcb1f3112d9f76f9159e9212128981
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030100"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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