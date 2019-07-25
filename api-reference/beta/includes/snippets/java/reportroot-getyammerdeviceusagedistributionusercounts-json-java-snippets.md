---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a7e7c5db7d81a958c3435fe90abafb4d4064fbd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871433"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageDistributionUserCountsCollectionPage getYammerDeviceUsageDistributionUserCounts = graphClient.reports()
    .getYammerDeviceUsageDistributionUserCounts('D7')
    .buildRequest()
    .get();

```