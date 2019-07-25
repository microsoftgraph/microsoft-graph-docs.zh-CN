---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 372eb9c2b67c399a8624a9a2aab19c6cdb6ac438
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886334"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageUserDetail('D7')
    .buildRequest()
    .get();

```