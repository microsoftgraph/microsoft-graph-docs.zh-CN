---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac2369e35282c15b7eab795976d762bec5c3227b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.DetailsRequestBuilderPatchOptions{
    H: headers,
}
plannerPlanId := "plannerPlan-id"
graphClient.Planner().PlansById(&plannerPlanId).Details().Patch(options)


```