---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9b580c97148d6c379ab8b9a1891f6c60d671f45
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806059"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = new TokenLifetimePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenLifetimePolicy.definition = definitionList;
tokenLifetimePolicy.displayName = "displayName-value";
tokenLifetimePolicy.isOrganizationDefault = true;

graphClient.policies().tokenLifetimePolicies()
    .buildRequest()
    .post(tokenLifetimePolicy);

```