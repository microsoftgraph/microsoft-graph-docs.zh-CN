---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d53c12d160cb4e3966151b0cd7e73509a2b6eb4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092505"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerPlanId := "plannerPlan-id"
result, err := graphClient.Planner().PlansById(&plannerPlanId).Details().Get(options)


```