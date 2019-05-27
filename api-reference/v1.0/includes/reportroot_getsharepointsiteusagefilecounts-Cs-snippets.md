---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83a0b5d4759c9a6d153acc8f3128401c6d60a912
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsageFileCounts('D7')
    .Request()
    .GetAsync();

```