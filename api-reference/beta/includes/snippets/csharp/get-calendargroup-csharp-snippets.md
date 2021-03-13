---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5e10ed26a11058f848d9b28601dcb6b257a8d9d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = await graphClient.Me.CalendarGroups["{calendarGroup-id}"]
    .Request()
    .GetAsync();

```