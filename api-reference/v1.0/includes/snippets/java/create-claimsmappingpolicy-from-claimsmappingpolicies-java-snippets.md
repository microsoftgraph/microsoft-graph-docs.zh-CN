---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ed3c66f4e02badd7ee3b801ae5fbf53456823c7916d264a7c1c25ac1cc14bfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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