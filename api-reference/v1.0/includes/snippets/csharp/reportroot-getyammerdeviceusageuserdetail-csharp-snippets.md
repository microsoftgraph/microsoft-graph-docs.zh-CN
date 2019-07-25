---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba17c685dd29140eb669aa3d18c9612f885f7fce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```