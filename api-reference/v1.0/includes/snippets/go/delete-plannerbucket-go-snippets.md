---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35fc699323ec1a1743dd0b014af343f36ade8bbd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerBucketRequestBuilderDeleteOptions{
    H: headers,
}
plannerBucketId := "plannerBucket-id"
graphClient.Planner().BucketsById(&plannerBucketId).Delete(options)


```