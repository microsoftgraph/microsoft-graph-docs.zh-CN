---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63fae4864d7e0637159e143e55be1fc7de6183bb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096063"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerPlan()
title := "title-value"
requestBody.SetTitle(&title)
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerPlanRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerPlanId := "plannerPlan-id"
graphClient.Planner().PlansById(&plannerPlanId).Patch(options)


```