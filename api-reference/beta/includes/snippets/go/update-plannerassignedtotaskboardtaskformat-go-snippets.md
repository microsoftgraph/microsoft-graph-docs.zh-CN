---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4e6316c661c2a2904d152e6ac3ccc49d3e8927f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325850"
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
options := &msgraphsdk.AssignedToTaskBoardFormatRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).AssignedToTaskBoardFormat().PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```