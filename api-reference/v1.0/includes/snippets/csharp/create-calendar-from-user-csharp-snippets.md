---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94b695b180ca740cef532229f783858e3ad807973e37aaf3b68d3c690373fc67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Volunteer"
};

await graphClient.Me.Calendars
    .Request()
    .AddAsync(calendar);

```