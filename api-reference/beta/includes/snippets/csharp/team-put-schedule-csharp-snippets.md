---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1079684b3063183e2e93b2ceb9b7e899e2d186b8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = new Schedule
{
    Enabled = true,
    TimeZone = "America/Chicago"
};

await graphClient.Teams["{teamId}"].Schedule
    .Request()
    .PutAsync(schedule);

```