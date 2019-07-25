---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9db7d1e8565ac25c6ffbbcbd819713eae9342d83
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value",
    ClassId = "classId-value",
    ChangeKey = "changeKey-value"
};

await graphClient.Me.CalendarGroups
    .Request()
    .AddAsync(calendarGroup);

```