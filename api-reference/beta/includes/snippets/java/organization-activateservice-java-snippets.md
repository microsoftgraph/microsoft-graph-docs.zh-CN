---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8e0be0c63bf6f43779cdd37f7ff8e9dfa4f82f9655939ab20480fbaf3c11db7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333144"
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