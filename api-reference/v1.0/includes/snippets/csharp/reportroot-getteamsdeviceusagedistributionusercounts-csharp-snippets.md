---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 70cc8d308dd0362487b639d57eb2cb6ce27dab3c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```