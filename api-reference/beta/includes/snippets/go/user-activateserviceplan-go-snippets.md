---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4558610ad002ccc3b18508861c6199de09e173d1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100250"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
servicePlanId := "28f42d6f-8034-4a0f-9d8a-a218a63b3299"
requestBody.SetServicePlanId(&servicePlanId)
skuId := "465a2a90-5e59-456d-a7b8-127b9fb2e484"
requestBody.SetSkuId(&skuId)
options := &msgraphsdk.ActivateServicePlanRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Me().ActivateServicePlan().Post(options)


```