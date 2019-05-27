---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cabfde47d95071917c30e03557d25075e28ac99f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480454"
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