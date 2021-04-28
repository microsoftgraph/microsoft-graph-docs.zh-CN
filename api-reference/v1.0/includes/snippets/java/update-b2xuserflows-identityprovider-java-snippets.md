---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 477693ff03ddffa4d7334594b5dfd2a1df77fb8a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProviders = new IdentityProvider();
identityProviders.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"));

graphClient.identity().b2xUserFlows("B2X_1_Partner").identityProviders().references()
    .buildRequest()
    .patch(identityProviders);

```