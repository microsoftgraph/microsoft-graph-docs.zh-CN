---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d07cad22df2532d93ad37ebfe0b8593d5b7e4712
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863932"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy();
homeRealmDiscoveryPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.servicePrincipals("{id}").homeRealmDiscoveryPolicies().references()
    .buildRequest()
    .post(homeRealmDiscoveryPolicy);

```