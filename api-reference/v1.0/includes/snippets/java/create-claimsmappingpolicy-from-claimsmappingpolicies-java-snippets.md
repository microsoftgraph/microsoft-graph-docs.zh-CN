---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c29864b5652331c8a04f8d867f4ebc5a5d15123e
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
claimsMappingPolicy.definition = definitionList;
claimsMappingPolicy.displayName = "displayName-value";
claimsMappingPolicy.isOrganizationDefault = true;

graphClient.policies().claimsMappingPolicies()
    .buildRequest()
    .post(claimsMappingPolicy);

```