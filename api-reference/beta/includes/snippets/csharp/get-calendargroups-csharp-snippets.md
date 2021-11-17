---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e555e2764323a6b3c6188c4cba3af1cf26e162c163da5cfa6ebd16b689bb9cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333625"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroups = await graphClient.Me.CalendarGroups
    .Request()
    .GetAsync();

```