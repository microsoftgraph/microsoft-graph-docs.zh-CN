---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4bfb3ac1b274eac5bb5431f7b1e514eeb876786c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityCounts = await graphClient.Reports
    .GetTeamsUserActivityCounts('D7')
    .Request()
    .GetAsync();

```