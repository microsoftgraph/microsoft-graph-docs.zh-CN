---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de7b8bc61238475ab4a23cd9190fe36d300173c6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984218"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerBucket()
name := "Advertising"
requestBody.SetName(&name)
planId := "xqQg5FS2LkCp935s-FIFm2QAFkHM"
requestBody.SetPlanId(&planId)
orderHint := " !"
requestBody.SetOrderHint(&orderHint)
options := &msgraphsdk.BucketsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Buckets().Post(options)


```