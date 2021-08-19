---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2adee47dc406695f420fe51112b81007e854f0800ea80dda1450b84cb37bab55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162480"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.responseType = EnumSet.of(OpenIdConnectResponseTypes.ID_TOKEN);

graphClient.identityProviders("OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a")
    .buildRequest()
    .patch(identityProvider);

```