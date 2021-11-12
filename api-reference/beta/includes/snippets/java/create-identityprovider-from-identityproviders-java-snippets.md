---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17804c985007e103bc38a74f30d6946bbde848155704f42e0e385fa3408674b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333030"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.name = "Login with Amazon";
identityProvider.type = "Amazon";
identityProvider.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
identityProvider.clientSecret = "000000000000";

graphClient.identityProviders()
    .buildRequest()
    .post(identityProvider);

```