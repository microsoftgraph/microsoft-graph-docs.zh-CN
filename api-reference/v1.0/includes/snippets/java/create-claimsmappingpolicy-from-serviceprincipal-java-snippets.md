---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bf39a3d86189bbb64283eb870da766dddc2e218
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981371"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
claimsMappingPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.servicePrincipals("{id}").claimsMappingPolicies().references()
    .buildRequest()
    .post(claimsMappingPolicy);

```