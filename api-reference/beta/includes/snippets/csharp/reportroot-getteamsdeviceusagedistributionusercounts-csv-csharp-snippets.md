---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d3b56f125c3e6c226e27b73aceae3d4f2f170c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageDistributionUserCounts = await graphClient.Reports
    .GetTeamsDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```