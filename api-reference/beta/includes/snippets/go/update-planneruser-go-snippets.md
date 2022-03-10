---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 614a0bf5f314db129254a36f4f10258785e60a73
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412497"
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
options := &msgraphsdk.PlannerRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Me().Planner().Patch(options)


```