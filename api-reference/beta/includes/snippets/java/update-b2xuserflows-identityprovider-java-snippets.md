---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b5a9fd013b48facc5ed5bec30c9de5fec6591d3987f795a17877a6b37185116
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105885"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identityProviders/{id}"));

graphClient.identity().b2xUserFlows("{id}").identityProviders().references()
    .buildRequest()
    .post(identityProvider);

```