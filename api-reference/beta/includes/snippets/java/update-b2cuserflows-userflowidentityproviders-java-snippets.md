---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2632d0913fdebbae5fecec313b8e42638299755d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider userFlowIdentityProviders = new IdentityProvider();
userFlowIdentityProviders.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/identityProviders/{id}"));

graphClient.identity().b2cUserFlows("B2C_test_signin_signup").userFlowIdentityProviders().references()
    .buildRequest()
    .patch(userFlowIdentityProviders);

```