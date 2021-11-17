---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f2a74416b0b10baefac00995ce6e3ab4cf523b8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033920"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerAssignedToTaskBoardTaskFormat()
orderHintsByAssignee := msgraphsdk.NewPlannerOrderHintsByAssignee()
requestBody.SetOrderHintsByAssignee(orderHintsByAssignee)
orderHintsByAssignee.SetAdditionalData(map[string]interface{}{
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!",
}
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.AssignedToTaskBoardFormatRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).AssignedToTaskBoardFormat().Patch(options)


```