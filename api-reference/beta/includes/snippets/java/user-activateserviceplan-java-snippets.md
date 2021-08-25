---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ae600677f6371fad71fd9a7fc528ccbf3f43b5852113d0fb131443f2022a977
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279559"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID servicePlanId = UUID.fromString("28f42d6f-8034-4a0f-9d8a-a218a63b3299");

UUID skuId = UUID.fromString("465a2a90-5e59-456d-a7b8-127b9fb2e484");

graphClient.me()
    .activateServicePlan(UserActivateServicePlanParameterSet
        .newBuilder()
        .withServicePlanId(servicePlanId)
        .withSkuId(skuId)
        .build())
    .buildRequest()
    .post();

```