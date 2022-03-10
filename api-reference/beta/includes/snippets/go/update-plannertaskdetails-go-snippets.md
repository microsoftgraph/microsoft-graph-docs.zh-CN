---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2115df22d963579bd30882d477e5617985cb13f6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411806"
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
options := &msgraphsdk.DetailsRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerTaskId := "plannerTask-id"
result, err := graphClient.Planner().TasksById(&plannerTaskId).Details().Patch(options)


```