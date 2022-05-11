---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36e0dda44b659c8feda5dd1450f82ae301fd0964
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327438"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerUser()
favoritePlanReferences := msgraphsdk.NewPlannerFavoritePlanReferenceCollection()
requestBody.SetFavoritePlanReferences(favoritePlanReferences)
favoritePlanReferences.SetAdditionalData(map[string]interface{}{
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": nil,
}
recentPlanReferences := msgraphsdk.NewPlannerRecentPlanReferenceCollection()
requestBody.SetRecentPlanReferences(recentPlanReferences)
recentPlanReferences.SetAdditionalData(map[string]interface{}{
}
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=""
}
options := &msgraphsdk.PlannerRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
graphClient.Me().Planner().PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```