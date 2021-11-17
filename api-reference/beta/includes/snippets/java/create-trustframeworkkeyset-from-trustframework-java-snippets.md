---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e1898e563d750253cdfc5a2e22cabdad4b2e2e97246497e89749a419c9d568b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221503"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySet trustFrameworkKeySet = new TrustFrameworkKeySet();
trustFrameworkKeySet.id = "keyset1";
LinkedList<TrustFrameworkKey> keysList = new LinkedList<TrustFrameworkKey>();
TrustFrameworkKey keys = new TrustFrameworkKey();
keys.k = "k-value";
LinkedList<String> x5cList = new LinkedList<String>();
x5cList.add("x5c-value");
keys.x5c = x5cList;
keys.x5t = "x5t-value";
keys.kty = "kty-value";
keys.use = "use-value";
keys.exp = 99L;
keys.nbf = 99L;
keys.kid = "kid-value";
keys.e = "e-value";
keys.n = "n-value";
keys.d = "d-value";
keys.p = "p-value";
keys.q = "q-value";
keys.dp = "dp-value";
keys.dq = "dq-value";
keys.qi = "qi-value";
keysList.add(keys);
trustFrameworkKeySet.keys = keysList;

graphClient.trustFramework().keySets()
    .buildRequest()
    .post(trustFrameworkKeySet);

```