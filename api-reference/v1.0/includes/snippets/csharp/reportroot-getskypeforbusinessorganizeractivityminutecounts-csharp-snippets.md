---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c675f91f192c282dc237387031094c1d3bb6395c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```