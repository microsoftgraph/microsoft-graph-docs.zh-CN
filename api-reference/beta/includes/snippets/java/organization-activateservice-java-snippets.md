---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33c514e535e4494903e350a0c1623d6f215dccf9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID skuId = UUID.fromString("6fd2c87f-b296-42f0-b197-1e91e994b900");

UUID servicePlanId = UUID.fromString("a23b959c-7ce8-4e57-9140-b90eb88a9e97");

graphClient.organization("{:organizationId}")
    .activateService(OrganizationActivateServiceParameterSet
        .newBuilder()
        .withService(null)
        .withServicePlanId(servicePlanId)
        .withSkuId(skuId)
        .build())
    .buildRequest()
    .post();

```