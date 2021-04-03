---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f88e8018eec04e02ea54f1dc66676da538df7d5
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506992"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "Personal events"
};

await graphClient.Me.CalendarGroups
    .Request()
    .AddAsync(calendarGroup);

```