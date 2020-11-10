---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae7950bc083a14f29ca037ac3129a56e2b136c86
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980926"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySet trustFrameworkKeySet = new TrustFrameworkKeySet();
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

graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .put(trustFrameworkKeySet);

```