---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1409e2e4219de38ef33d7ebbf0a552b42390a6e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageDistributionUserCounts = await graphClient.Reports.GetYammerDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```