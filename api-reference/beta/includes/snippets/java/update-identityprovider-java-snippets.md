---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de8df7c2ce5d4d69bcd2e8eeb8edba6344ef3adb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857576"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.clientSecret = "1111111111111";

graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .patch(identityProvider);

```