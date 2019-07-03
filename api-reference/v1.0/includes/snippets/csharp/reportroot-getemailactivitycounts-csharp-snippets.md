---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f82253a9feb233ee0042c3928cdcf3c593051e51
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493165"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailActivityCounts('D7')
    .Request()
    .GetAsync();

```