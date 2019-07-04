---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 940ac47faa59cdd42dafd03637bb8931454ca314
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .SkipToken("R0usmci39OQxqJrxK4")
    .GetAsync();

```