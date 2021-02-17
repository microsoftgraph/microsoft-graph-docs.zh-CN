---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17a68627df75b011409c9da860b09ec00d1450c8
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRosterMember = await graphClient.Planner.Rosters["523a9d5a-f9d5-45c1-929f-b8525393515c"].Members["5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38"]
    .Request()
    .GetAsync();

```