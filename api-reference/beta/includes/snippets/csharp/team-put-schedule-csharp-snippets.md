---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1079684b3063183e2e93b2ceb9b7e899e2d186b8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617058"
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