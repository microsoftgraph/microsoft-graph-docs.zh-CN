---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad8642fa8ff4b2b2cd4ee5c84f6763afa83ea444
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985513"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerPlan()
container := msgraphsdk.NewPlannerPlanContainer()
requestBody.SetContainer(container)
url := "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
container.SetUrl(&url)
title := "title-value"
requestBody.SetTitle(&title)
options := &msgraphsdk.PlansRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Plans().Post(options)


```