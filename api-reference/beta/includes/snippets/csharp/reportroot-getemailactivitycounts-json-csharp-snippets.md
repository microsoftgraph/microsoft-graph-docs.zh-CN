---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b341bcce1e229e5fea1a7d549215ca835f2133e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874064"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityCounts = await graphClient.Reports
    .GetEmailActivityCounts('D7')
    .Request()
    .GetAsync();

```