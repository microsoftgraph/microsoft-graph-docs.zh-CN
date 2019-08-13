---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e9b526ed0790080bba64d96d9732247f460f4d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320420"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsUserActivityUserCounts("D7")
    .Request()
    .GetAsync();

```