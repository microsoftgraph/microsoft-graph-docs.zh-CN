---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39a60fdec7ddf881645be2aa65875e73407ae159
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985464"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerTask()
planId := "xqQg5FS2LkCp935s-FIFm2QAFkHM"
requestBody.SetPlanId(&planId)
bucketId := "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
requestBody.SetBucketId(&bucketId)
title := "Update client list"
requestBody.SetTitle(&title)
assignments := msgraphsdk.NewPlannerAssignments()
requestBody.SetAssignments(assignments)
assignments.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Tasks().Post(options)


```