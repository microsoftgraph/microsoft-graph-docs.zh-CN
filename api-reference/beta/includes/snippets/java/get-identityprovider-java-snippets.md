---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95f6760a042351ac0b32b2ef5ed4af4ccb4fe865
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .get();

```