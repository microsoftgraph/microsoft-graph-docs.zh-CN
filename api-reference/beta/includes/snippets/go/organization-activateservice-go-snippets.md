---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 266034c6801507a26f5413ae7581c833c89b3756
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412500"
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
graphClient.OrganizationById(&organizationId).ActivateService(organization-id).Post(options)


```