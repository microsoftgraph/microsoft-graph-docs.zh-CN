---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 798d697598ece702ad7215bce826b963eec8ee96
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084265"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerPlanId := "plannerPlan-id"
result, err := graphClient.Planner().PlansById(&plannerPlanId).Buckets().Get(options)


```