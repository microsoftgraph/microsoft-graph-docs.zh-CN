---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a9721cb3dc176c5292ab840efe9d3fae27eb201
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799202"
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