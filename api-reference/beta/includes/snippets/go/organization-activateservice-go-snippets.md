---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab883eac255c9b0d718855bb66b165a0e28f382f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082815"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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