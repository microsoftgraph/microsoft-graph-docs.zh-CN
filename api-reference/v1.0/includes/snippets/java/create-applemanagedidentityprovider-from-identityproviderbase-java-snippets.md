---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9e27056f3f96f04e485824fb6ecc891015f1313
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppleManagedIdentityProvider identityProviderBase = new AppleManagedIdentityProvider();
identityProviderBase.displayName = "Sign in with Apple";
identityProviderBase.developerId = "UBF8T346G9";
identityProviderBase.serviceId = "com.microsoft.rts.b2c.test.client";
identityProviderBase.keyId = "99P6D879C4";
identityProviderBase.certificateData = "******";

graphClient.identity().identityProviders()
    .buildRequest()
    .post(identityProviderBase);

```