---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 167a47b4a85c0826d8e892373a0750cad2f6fffc
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
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