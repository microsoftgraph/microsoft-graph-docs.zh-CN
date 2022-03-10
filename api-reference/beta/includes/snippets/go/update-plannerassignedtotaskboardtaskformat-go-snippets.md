---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4490c955d1cadbe0104cc209ea769cc9e24a71a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411808"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
result, err := graphClient.Planner().TasksById(&plannerTaskId).AssignedToTaskBoardFormat().Patch(options)


```