---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1fc4c927674a9bad6d4c594c1f57c96359d3ab92
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889951"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean disableUserAccounts = True;

graphClient.domains("{id}")
    .forceDelete(disableUserAccounts)
    .buildRequest()
    .post();

```