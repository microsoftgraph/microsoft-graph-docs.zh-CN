---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08c8b9043c0dc3816ee1d781948beedd1026a0b4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091731"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerBucket()
name := "Development"
requestBody.SetName(&name)
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerBucketRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerBucketId := "plannerBucket-id"
graphClient.Planner().BucketsById(&plannerBucketId).Patch(options)


```