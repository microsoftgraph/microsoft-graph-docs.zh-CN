---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 855e9ca0772d16b9317c96ee36f3a8f1571cf2a8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979660"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
claimsMappingPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.servicePrincipals("{id}").claimsMappingPolicies().references()
    .buildRequest()
    .post(claimsMappingPolicy);

```