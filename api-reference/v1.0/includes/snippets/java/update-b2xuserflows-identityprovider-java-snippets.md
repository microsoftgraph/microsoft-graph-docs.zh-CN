---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59dafeb91c2aa1e2a739c02d1ccccb34d17c5e4c
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081586"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"));

graphClient.identity().b2xUserFlows("B2X_1_Partner").identityProviders().references()
    .buildRequest()
    .post(identityProvider);

```