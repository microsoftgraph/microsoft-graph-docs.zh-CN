---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88f35d11cfb237022774242c446a3c48a081f783
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351186"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("{"HomeRealmDiscoveryPolicy":
     {"AccelerateToFederatedDomain":true,
      "PreferredDomain":"federated.example.edu",
      "AlternateIdLogin":{"Enabled":true}}}");
homeRealmDiscoveryPolicy.definition = definitionList;
homeRealmDiscoveryPolicy.displayName = "Contoso default HRD Policy";

graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .patch(homeRealmDiscoveryPolicy);

```