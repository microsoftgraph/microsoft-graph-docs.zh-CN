---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35dd2549840da20a6be6c5ad7a65793022b74f59ed32dc7121a9a4792bd83329
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162981"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicyCollectionPage homeRealmDiscoveryPolicies = graphClient.policies().homeRealmDiscoveryPolicies()
    .buildRequest()
    .get();

```