---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cabfde47d95071917c30e03557d25075e28ac99f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notifyTeam = true;

var startDateTime = 10/8/2018 12:00:00 AM;

var endDateTime = 10/15/2018 12:00:00 AM;

await graphClient.Teams["{teamId}"].Schedule
    .Share(notifyTeam,startDateTime,endDateTime)
    .Request()
    .PostAsync();

```