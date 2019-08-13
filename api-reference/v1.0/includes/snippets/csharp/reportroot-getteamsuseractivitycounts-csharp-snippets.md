---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e791d4a4fc3b88b719ffad11ad9e7b89838b8db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsUserActivityCounts("D7")
    .Request()
    .GetAsync();

```