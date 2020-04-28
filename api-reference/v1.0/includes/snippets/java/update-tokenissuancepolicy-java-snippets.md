---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d1fa5d8e726cac2d1392da4acd699baacafc077
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719457"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicy tokenIssuancePolicy = new TokenIssuancePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenIssuancePolicy.definition = definitionList;
tokenIssuancePolicy.displayName = "displayName-value";
tokenIssuancePolicy.isOrganizationDefault = true;
tokenIssuancePolicy.type = "type-value";

graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .patch(tokenIssuancePolicy);

```