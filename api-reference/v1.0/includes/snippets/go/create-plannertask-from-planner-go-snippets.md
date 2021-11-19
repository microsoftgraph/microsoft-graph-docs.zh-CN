---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b724a4443fce5c2f665f08702da917550361fb5e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099141"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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