---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5d28bf3a5387db35760f3b28b305fce24747e4af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityCounts("D7")
    .Request()
    .GetAsync();

```