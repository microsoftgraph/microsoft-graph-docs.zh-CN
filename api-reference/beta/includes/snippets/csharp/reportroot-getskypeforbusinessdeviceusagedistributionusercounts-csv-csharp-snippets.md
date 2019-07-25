---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 30f09cbea35f1d93979a02dc277a663b9a1ebb27
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageDistributionUserCounts = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```