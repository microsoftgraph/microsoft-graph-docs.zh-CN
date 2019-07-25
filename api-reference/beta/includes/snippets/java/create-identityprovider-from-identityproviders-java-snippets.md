---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 92548f7d07463e5919eb8e57e99f77ee35833f08
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857581"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.name = "Login with Amazon";
identityProvider.type = "Amazon";
identityProvider.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
identityProvider.clientSecret = "000000000000";

graphClient.identityProviders()
    .buildRequest()
    .post(identityProvider);

```