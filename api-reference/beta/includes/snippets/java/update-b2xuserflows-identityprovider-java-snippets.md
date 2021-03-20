---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7b25db9a1f0a59280148176fe801a42235bb1c8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976410"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProviders = new IdentityProvider();
identityProviders.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identityProviders/{id}"));

graphClient.identity().b2xUserFlows("{id}").identityProviders().references()
    .buildRequest()
    .patch(identityProviders);

```