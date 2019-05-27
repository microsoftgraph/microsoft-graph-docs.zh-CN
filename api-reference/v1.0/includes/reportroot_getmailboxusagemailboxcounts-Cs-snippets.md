---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 636008c94ea5c339accc3645164b521eb76c1e2c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageMailboxCounts('D7')
    .Request()
    .GetAsync();

```