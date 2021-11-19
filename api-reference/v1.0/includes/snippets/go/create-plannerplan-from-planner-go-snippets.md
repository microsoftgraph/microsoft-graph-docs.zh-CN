---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49de421b85c37845078908d3fa47eb39ca09ba1c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100115"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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