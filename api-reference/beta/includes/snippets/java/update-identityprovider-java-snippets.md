---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15a37b7934e55e15a5e39b65601562fd8982ad98
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.clientSecret = "1111111111111";

graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .patch(identityProvider);

```