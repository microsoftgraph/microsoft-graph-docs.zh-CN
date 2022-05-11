---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b0d17ca2102ab5eca37a7ce0adfcc7ef83ceb5b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328075"
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
options := &msgraphsdk.DetailsRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
plannerPlanId := "plannerPlan-id"
graphClient.Planner().PlansById(&plannerPlanId).Details().PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```