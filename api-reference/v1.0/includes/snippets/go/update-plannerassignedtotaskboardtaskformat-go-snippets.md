---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fad25e327031e5a00e5e9f972aab72ca8bceb0e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082773"
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
graphClient.Planner().TasksById(&plannerTaskId).AssignedToTaskBoardFormat().Patch(options)


```