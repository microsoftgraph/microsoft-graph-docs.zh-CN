---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 454b5b4e2096e0de5f937f634d8fc145fbb983ee
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53578740"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SocialIdentityProvider identityProviderBase = new SocialIdentityProvider();
identityProviderBase.displayName = "Login with Amazon";
identityProviderBase.identityProviderType = "Amazon";
identityProviderBase.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
identityProviderBase.clientSecret = "000000000000";

graphClient.identity().identityProviders()
    .buildRequest()
    .post(identityProviderBase);

```