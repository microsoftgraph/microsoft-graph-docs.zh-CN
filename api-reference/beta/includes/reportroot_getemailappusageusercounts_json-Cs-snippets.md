---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05e3192174d0688c090d0570f2f9fb76c7e37400
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserCounts = await graphClient.Reports.GetEmailAppUsageUserCounts('D7')
    .Request()
    .GetAsync();

```