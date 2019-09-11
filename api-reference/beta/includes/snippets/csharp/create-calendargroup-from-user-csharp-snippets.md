---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b996354bf56fb2b8e5cc652eea69af64394538b0
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value",
    ClassId = Guid.Parse("classId-value"),
    ChangeKey = "changeKey-value"
};

await graphClient.Me.CalendarGroups
    .Request()
    .AddAsync(calendarGroup);

```