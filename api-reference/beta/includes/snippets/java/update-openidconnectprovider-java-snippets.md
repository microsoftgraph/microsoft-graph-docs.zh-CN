---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fea4b6cf22659ea0952479f975c2c8ea9cfd40d4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SocialIdentityProvider identityProviderBase = new SocialIdentityProvider();
identityProviderBase.responseType = EnumSet.of(OpenIdConnectResponseTypes.ID_TOKEN);

graphClient.identity().identityProviders("OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7")
    .buildRequest()
    .patch(identityProviderBase);

```