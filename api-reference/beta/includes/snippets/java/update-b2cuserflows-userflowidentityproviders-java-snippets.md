---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88917e06bd7c78b4a7ea83fd55951686c0bed699
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439676"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase userFlowIdentityProviders = new IdentityProviderBase();
userFlowIdentityProviders.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/identityProviders/{id}"));

graphClient.identity().b2cUserFlows("B2C_test_signin_signup").userFlowIdentityProviders().references()
    .buildRequest()
    .patch(userFlowIdentityProviders);

```