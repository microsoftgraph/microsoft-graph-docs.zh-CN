---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb153e97ed85e969fc30ce69ec9928602a5ac15c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014431"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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