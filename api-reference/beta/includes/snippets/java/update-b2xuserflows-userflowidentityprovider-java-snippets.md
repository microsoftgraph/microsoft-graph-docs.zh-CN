---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c37f7df76bd82cde2d9e3bad87d980c62d0a12e2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368876"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider userFlowIdentityProviders = new IdentityProvider();
userFlowIdentityProviders.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"));

graphClient.identity().b2xUserFlows("B2X_1_Test").userFlowIdentityProviders().references()
    .buildRequest()
    .patch(userFlowIdentityProviders);

```