---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e56fac2d080a2db09bdc917eff114780e45ef274
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321835"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityUserCounts("D7")
    .Request()
    .GetAsync();

```