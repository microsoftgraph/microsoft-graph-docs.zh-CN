---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d751595e7fa67eeac0a1368d8e081120b8383d8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328391"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerTaskDetails()
previewType := "noPreview"
requestBody.SetPreviewType(&previewType)
references := msgraphsdk.NewPlannerExternalReferences()
requestBody.SetReferences(references)
references.SetAdditionalData(map[string]interface{}{
    "http%3A//www%2Ebing%2Ecom": nil,
}
checklist := msgraphsdk.NewPlannerChecklistItems()
requestBody.SetChecklist(checklist)
checklist.SetAdditionalData(map[string]interface{}{
    "a93c93c5-10a6-4167-9551-8bafa09967a7": nil,
}
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.DetailsRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).Details().PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```