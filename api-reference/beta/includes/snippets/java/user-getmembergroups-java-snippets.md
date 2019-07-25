---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddd1dae849fccaaedba1931034e33f08e11c62fc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.me()
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```