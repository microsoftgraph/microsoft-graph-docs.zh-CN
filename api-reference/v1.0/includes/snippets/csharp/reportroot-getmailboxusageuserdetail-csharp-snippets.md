---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 940d4ba5eaf3384db2bb175f64512ada74338bd7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageDetail('D7')
    .Request()
    .GetAsync();

```