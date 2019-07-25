---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 181abb20207fa20dc321d894fc376e481552f48f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891808"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityUserCounts('D7')
    .buildRequest()
    .get();

```