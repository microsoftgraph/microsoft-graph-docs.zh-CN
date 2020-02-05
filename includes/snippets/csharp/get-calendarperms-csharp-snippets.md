---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f6475067ac467f9e83f14f8e8b0f247b88b0528
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774785"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermissions = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendar.CalendarPermissions
    .Request()
    .GetAsync();

```