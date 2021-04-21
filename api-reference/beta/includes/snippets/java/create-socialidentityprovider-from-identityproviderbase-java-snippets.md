---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 454b5b4e2096e0de5f937f634d8fc145fbb983ee
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921323"
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