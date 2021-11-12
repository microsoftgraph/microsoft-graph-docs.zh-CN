---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b577c98eb438cac590b05e489263f2797f90960f6f871db0eb83223abae9521
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identityProviders/{id}"));

graphClient.identity().b2cUserFlows("{id}").identityProviders().references()
    .buildRequest()
    .post(identityProvider);

```