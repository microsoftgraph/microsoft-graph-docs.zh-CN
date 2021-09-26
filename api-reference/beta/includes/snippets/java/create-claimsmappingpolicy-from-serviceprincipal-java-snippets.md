---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75a8b3c4c8f8ddb0638642ef6036255541b89ca0
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
claimsMappingPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.servicePrincipals("{servicePrincipal-id}").claimsMappingPolicies().references()
    .buildRequest()
    .post(claimsMappingPolicy);

```