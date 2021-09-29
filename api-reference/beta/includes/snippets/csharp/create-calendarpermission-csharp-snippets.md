---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddd9f512e92e051732a1f44139bbbbc6e85bf634
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    EmailAddress = new EmailAddress
    {
        Name = "Samantha Booth",
        Address = "samanthab@adatum.onmicrosoft.com"
    },
    IsInsideOrganization = true,
    IsRemovable = true,
    Role = CalendarRoleType.Read
};

await graphClient.Users["{user-id}"].Calendar.CalendarPermissions
    .Request()
    .AddAsync(calendarPermission);

```