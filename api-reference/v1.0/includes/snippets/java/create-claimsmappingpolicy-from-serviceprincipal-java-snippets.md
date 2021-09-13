---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc8d8ecb637b0ba5e04e0e79fa507cd237030f34171afe12f3f79a6c9d994f25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162352"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
claimsMappingPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.servicePrincipals("{id}").claimsMappingPolicies().references()
    .buildRequest()
    .post(claimsMappingPolicy);

```