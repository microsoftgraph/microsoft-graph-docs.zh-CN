---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 81d4af4caddfbe7a25a325888f78801888f68e79
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```