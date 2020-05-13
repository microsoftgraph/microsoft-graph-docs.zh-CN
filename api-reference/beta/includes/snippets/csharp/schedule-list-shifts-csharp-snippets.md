---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7a49d4220d24220a0079187b5a4c274d3902a72
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35725662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shifts = await graphClient.Teams["{teamId}"].Schedule.Shifts
    .Request()
    .Filter("sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```