---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9adf0c4796daa200bc62be1e59dd239e44f3e74
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroup = await graphClient.Teams["{teamId}"].Schedule.SchedulingGroups["{schedulingGroupId}"]
    .Request()
    .GetAsync();

```