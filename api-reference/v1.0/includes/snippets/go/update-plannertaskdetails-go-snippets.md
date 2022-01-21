---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee1d71787e7aa5a1538707b53f01b34bdb01026b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135812"
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
graphClient.Planner().TasksById(&plannerTaskId).Details().Patch(options)


```