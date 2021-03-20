---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc36dec95936266a7e3a169d3cc20265a559e68e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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