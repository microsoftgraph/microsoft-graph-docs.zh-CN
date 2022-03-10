---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0357bdcb1a51f37498442569ac2eb7404a23353b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412726"
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
result, err := graphClient.Planner().PlansById(&plannerPlanId).Details().Patch(options)


```