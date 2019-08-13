---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6667c88a1608b167f1724c0ca608036dde8ac607
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageFileCounts = await graphClient.Reports
    .GetOneDriveUsageFileCounts("D7")
    .Request()
    .GetAsync();

```