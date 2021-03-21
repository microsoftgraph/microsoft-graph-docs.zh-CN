---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0762d12b2309c29eaa20f7096f2193c2234d1da3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String use = "sig";

String kty = "RSA";

Long nbf = 1508969811L;

Long exp = 1508969811L;

graphClient.trustFramework().keySets("{id}")
    .generateKey(TrustFrameworkKeySetGenerateKeyParameterSet
        .newBuilder()
        .withUse(use)
        .withKty(kty)
        .withNbf(nbf)
        .withExp(exp)
        .build())
    .buildRequest()
    .post();

```