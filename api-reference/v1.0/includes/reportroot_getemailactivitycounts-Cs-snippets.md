---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f82253a9feb233ee0042c3928cdcf3c593051e51
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailActivityCounts('D7')
    .Request()
    .GetAsync();

```