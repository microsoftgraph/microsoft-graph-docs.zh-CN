---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f345228c4fbc4267597bd124eeb5db687bb5025b95437cfe9517ab319c6ae87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163419"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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