---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e5d7fa222a10d3cbeed104696b03cbdd2121ac2468a992a9f095cb4c3f2e0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274310"
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