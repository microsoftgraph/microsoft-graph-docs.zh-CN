---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6da481dff5a46e6723d163ca8d7f0ae02cbf103
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41778038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    Role = CalendarRoleType.Write
};

await graphClient.Users["{id}"].Calendar.CalendarPermissions["RGVmYXVsdA=="]
    .Request()
    .UpdateAsync(calendarPermission);

```