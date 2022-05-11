---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 688c298ef902675c30c2c1a025adfa8de0d5e10a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328486"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
skuId := "6fd2c87f-b296-42f0-b197-1e91e994b900"
requestBody.SetSkuId(&skuId)
servicePlanId := "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
requestBody.SetServicePlanId(&servicePlanId)
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).ActivateService(organization-id).Post(requestBody)


```