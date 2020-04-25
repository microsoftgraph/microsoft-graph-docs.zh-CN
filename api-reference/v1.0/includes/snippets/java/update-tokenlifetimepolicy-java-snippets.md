---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e77a9fd82f7a65015916c0e035a049915e13a7cf
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806040"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = new TokenLifetimePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenLifetimePolicy.definition = definitionList;
tokenLifetimePolicy.displayName = "displayName-value";
tokenLifetimePolicy.isOrganizationDefault = true;
tokenLifetimePolicy.type = "type-value";

graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .patch(tokenLifetimePolicy);

```