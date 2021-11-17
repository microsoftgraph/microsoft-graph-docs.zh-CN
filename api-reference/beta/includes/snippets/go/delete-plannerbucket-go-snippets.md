---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 530f7df07a16ac9c581ba4a39a13e0d468e014c7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033892"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerBucketRequestBuilderDeleteOptions{
    H: headers,
}
plannerBucketId := "plannerBucket-id"
graphClient.Planner().BucketsById(&plannerBucketId).Delete(options)


```