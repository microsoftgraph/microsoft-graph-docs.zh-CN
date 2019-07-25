---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f9a2a0f07f72f3f6a347ba31c2b93a1118e3450b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867571"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .invalidateAllRefreshTokens()
    .buildRequest()
    .post();

```