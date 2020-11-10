---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46e347888a4ff76011bdd3a664888c84fe1f54eb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953349"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.responseType = EnumSet.of(OpenIdConnectResponseTypes.ID_TOKEN);

graphClient.identityProviders("OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a")
    .buildRequest()
    .patch(identityProvider);

```