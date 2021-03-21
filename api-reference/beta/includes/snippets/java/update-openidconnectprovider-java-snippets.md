---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc4f70a3b577d0fa8bc80e9cfc876440640e4fc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966535"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.responseType = EnumSet.of(OpenIdConnectResponseTypes.ID_TOKEN);

graphClient.identityProviders("OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a")
    .buildRequest()
    .patch(identityProvider);

```