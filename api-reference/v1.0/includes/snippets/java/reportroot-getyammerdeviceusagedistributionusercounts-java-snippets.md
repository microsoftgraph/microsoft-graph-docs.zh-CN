---
description: 自动生成的文件。 不修改
ms.openlocfilehash: abe5d1572be101f374ab35ace7446dfa60150940
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885939"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerDeviceUsageDistributionUserCounts('D7')
    .buildRequest()
    .get();

```