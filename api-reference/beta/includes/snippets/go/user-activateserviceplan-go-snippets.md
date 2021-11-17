---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58eb671c754170822e30ad440bc6c79f7cd69d48
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031457"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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