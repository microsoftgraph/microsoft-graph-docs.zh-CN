---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d04871c08cbdf66c9c2b7151e5fc1ec631c2adf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326820"
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
options := &msgraphsdk.PlannerTaskRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```