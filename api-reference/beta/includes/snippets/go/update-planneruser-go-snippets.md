---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2200048cd21cc3e54c8ccc7a0f1af1b5d4ae27fc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021634"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Me().Planner().Patch(options)


```