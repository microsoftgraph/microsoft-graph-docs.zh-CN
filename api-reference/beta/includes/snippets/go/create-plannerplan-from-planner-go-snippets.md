---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2963d553910cdbe732e046a9d37aea306a3a893
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101158"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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