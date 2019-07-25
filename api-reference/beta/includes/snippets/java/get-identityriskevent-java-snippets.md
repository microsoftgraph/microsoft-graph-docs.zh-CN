---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bbef70d7ebc171462d35fae64d4713a4df747e75
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857541"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityRiskEvent identityRiskEvent = graphClient.identityRiskEvents("ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98")
    .buildRequest()
    .get();

```