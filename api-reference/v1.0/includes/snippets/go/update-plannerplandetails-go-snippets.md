---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd37aa5aac75a181fbb754de2789cb2839bc12e2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117185"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerPlanDetails()
sharedWith := msgraphsdk.NewPlannerUserIds()
requestBody.SetSharedWith(sharedWith)
sharedWith.SetAdditionalData(map[string]interface{}{
    "6463a5ce-2119-4198-9f2a-628761df4a62": true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a": false,
}
categoryDescriptions := msgraphsdk.NewPlannerCategoryDescriptions()
requestBody.SetCategoryDescriptions(categoryDescriptions)
category1 := "Indoors"
categoryDescriptions.SetCategory1(&category1)
categoryDescriptions.SetCategory3(nil)
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.DetailsRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerPlanId := "plannerPlan-id"
graphClient.Planner().PlansById(&plannerPlanId).Details().Patch(options)


```