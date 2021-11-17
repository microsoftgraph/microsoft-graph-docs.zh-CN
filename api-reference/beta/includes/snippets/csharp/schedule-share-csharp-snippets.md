---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db690ffe7200ea7a1089d8e24b9082b87fd510e06ac48e146874291e99243c94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158481"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notifyTeam = true;

var startDateTime = DateTimeOffset.Parse("2018-10-08T00:00:00Z");

var endDateTime = DateTimeOffset.Parse("2018-10-15T00:00:00Z");

await graphClient.Teams["{team-id}"].Schedule
    .Share(notifyTeam,startDateTime,endDateTime)
    .Request()
    .PostAsync();

```