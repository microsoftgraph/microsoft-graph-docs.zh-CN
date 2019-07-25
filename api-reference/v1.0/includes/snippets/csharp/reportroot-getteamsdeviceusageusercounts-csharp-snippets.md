---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a2aa71e1c11b74a3073f59dd1d1eb9eca0523c27
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```