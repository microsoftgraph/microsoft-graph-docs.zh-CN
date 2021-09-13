---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3535ee9ed7ff96224f3e387df2b77472bc3bdb777f103e5d70cc1e58c2b12900
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104345"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"));

graphClient.identity().b2xUserFlows("B2X_1_Partner").identityProviders().references()
    .buildRequest()
    .post(identityProvider);

```