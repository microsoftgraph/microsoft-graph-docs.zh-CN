---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d27212649d395513c839454a9d624d861906b19
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .SkipToken("R0usmcCM996atia_s")
    .GetAsync();

```