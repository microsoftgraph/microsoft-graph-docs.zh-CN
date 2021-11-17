---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66d3989caab604961e23c2bf8a2fade743856752
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027255"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerPlan()
owner := "ebf3b108-5234-4e22-b93d-656d7dae5874"
requestBody.SetOwner(&owner)
title := "title-value"
requestBody.SetTitle(&title)
options := &msgraphsdk.PlansRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Plans().Post(options)


```