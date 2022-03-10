---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f9597096fd05e8a9d9da1ffa7d06f66fd534e36
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412595"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerTask()
assignments := msgraphsdk.NewPlannerAssignments()
requestBody.SetAssignments(assignments)
assignments.SetAdditionalData(map[string]interface{}{
}
appliedCategories := msgraphsdk.NewPlannerAppliedCategories()
requestBody.SetAppliedCategories(appliedCategories)
appliedCategories.SetAdditionalData(map[string]interface{}{
    "category3": true,
    "category4": false,
}
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerTaskRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerTaskId := "plannerTask-id"
result, err := graphClient.Planner().TasksById(&plannerTaskId).Patch(options)


```