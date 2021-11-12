---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6fd174a99b82378f3bbe5e9cfc9c5b7bb5ba4228f103ec8b4c3c9c1f97ca3bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroup = await graphClient.Teams["{team-id}"].Schedule.SchedulingGroups["{schedulingGroup-id}"]
    .Request()
    .GetAsync();

```