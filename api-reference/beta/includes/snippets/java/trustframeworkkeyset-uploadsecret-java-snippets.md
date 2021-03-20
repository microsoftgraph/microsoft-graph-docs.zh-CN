---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56b29d065460b6338a2f9021794c0f7877306df6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972218"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String use = "use-value";

String k = "application-secret-to-be-uploaded";

Long nbf = 1508969811L;

Long exp = 1508973711L;

graphClient.trustFramework().keySets("{id}")
    .uploadSecret(TrustFrameworkKeySetUploadSecretParameterSet
        .newBuilder()
        .withUse(use)
        .withK(k)
        .withNbf(nbf)
        .withExp(exp)
        .build())
    .buildRequest()
    .post();

```