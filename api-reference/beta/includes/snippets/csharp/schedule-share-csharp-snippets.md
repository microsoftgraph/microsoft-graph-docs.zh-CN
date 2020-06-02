---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 167a47b4a85c0826d8e892373a0750cad2f6fffc
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "36845945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notifyTeam = true;

var startDateTime = DateTimeOffset.Parse("2018-10-08T00:00:00Z");

var endDateTime = DateTimeOffset.Parse("2018-10-15T00:00:00Z");

await graphClient.Teams["{teamId}"].Schedule
    .Share(notifyTeam,startDateTime,endDateTime)
    .Request()
    .PostAsync();

```