---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9e27056f3f96f04e485824fb6ecc891015f1313
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60938784"
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