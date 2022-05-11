---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5b2c298c906f8f7c2f6ccbef00e8a293464ef9c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328091"
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
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(requestBody)


```