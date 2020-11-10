---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5f6a5bb2568f187cdf4e22820943645c78fde85
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964732"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
homeRealmDiscoveryPolicy.definition = definitionList;
homeRealmDiscoveryPolicy.displayName = "displayName-value";
homeRealmDiscoveryPolicy.isOrganizationDefault = true;

graphClient.policies().homeRealmDiscoveryPolicies()
    .buildRequest()
    .post(homeRealmDiscoveryPolicy);

```