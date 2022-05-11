---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c609997274933f6351617e8a4902a8161603e000
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326360"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
servicePlanId := "28f42d6f-8034-4a0f-9d8a-a218a63b3299"
requestBody.SetServicePlanId(&servicePlanId)
skuId := "465a2a90-5e59-456d-a7b8-127b9fb2e484"
requestBody.SetSkuId(&skuId)
graphClient.Me().ActivateServicePlan().Post(requestBody)


```