---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bac3d93ee9972a484fd21e4e5c4da2808a0c3b0c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.CalendarGroups["{id}"].Calendars
    .Request()
    .GetAsync();

```