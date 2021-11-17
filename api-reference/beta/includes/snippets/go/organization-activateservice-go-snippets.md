---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa2bab8a2b5b11fe6351ac2e829141d2849b3d82
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985941"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
skuId := "6fd2c87f-b296-42f0-b197-1e91e994b900"
requestBody.SetSkuId(&skuId)
servicePlanId := "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
requestBody.SetServicePlanId(&servicePlanId)
options := &msgraphsdk.ActivateServiceRequestBuilderPostOptions{
    Body: requestBody,
}
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).ActivateService().Post(options)


```