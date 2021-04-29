---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ada5845bec80036d411e154cc9c4a3b8f7dde2dd
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081511"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identityProviders/{id}"));

graphClient.identity().b2xUserFlows("{id}").identityProviders().references()
    .buildRequest()
    .post(identityProvider);

```