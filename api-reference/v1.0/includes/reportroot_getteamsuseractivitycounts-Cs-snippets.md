---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c174be059e79b0654fd8fe6f1bfcc443cadd29eb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetTeamsUserActivityCounts('D7')
    .Request()
    .GetAsync();

```