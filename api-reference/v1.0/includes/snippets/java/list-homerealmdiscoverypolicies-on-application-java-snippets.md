---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c74ddf975fdfe57b8e67876a7022b0e03396f6e72c9f2bc33a846b04b28e08dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221384"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicyCollectionWithReferencesPage homeRealmDiscoveryPolicies = graphClient.servicePrincipals("{id}").homeRealmDiscoveryPolicies()
    .buildRequest()
    .get();

```