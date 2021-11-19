---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b4128a18339bf6f6c4fe03fd7de40b9ae8dae18
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101271"
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
graphClient.Me().Planner().Patch(options)


```