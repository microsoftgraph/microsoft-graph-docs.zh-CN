---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a5de80c7e2544e1957d818decc8c20b6d5732e8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327505"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerPlan()
owner := "ebf3b108-5234-4e22-b93d-656d7dae5874"
requestBody.SetOwner(&owner)
title := "title-value"
requestBody.SetTitle(&title)
result, err := graphClient.Planner().Plans().Post(requestBody)


```