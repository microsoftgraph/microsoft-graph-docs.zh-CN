---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 505d59a4b244d5c17037ae4a0af051dfb3e9e8f5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328534"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerBucket()
name := "Advertising"
requestBody.SetName(&name)
planId := "xqQg5FS2LkCp935s-FIFm2QAFkHM"
requestBody.SetPlanId(&planId)
orderHint := " !"
requestBody.SetOrderHint(&orderHint)
result, err := graphClient.Planner().Buckets().Post(requestBody)


```