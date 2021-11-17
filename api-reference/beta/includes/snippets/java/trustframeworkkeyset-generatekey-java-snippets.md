---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fe1bbbe1daa47259a588b6f70809d70e6d12a90c59971059bf008fa533175e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220062"
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