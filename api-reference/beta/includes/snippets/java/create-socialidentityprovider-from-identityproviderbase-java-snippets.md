---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ddd260fb86047c057d2cb4e3c53da59b946aa7cc32b6f2973f68e876ce52071
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105747"
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