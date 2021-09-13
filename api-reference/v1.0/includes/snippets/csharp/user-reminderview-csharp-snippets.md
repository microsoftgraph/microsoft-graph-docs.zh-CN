---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d1ac28cb15648ab488161897fb5af72f8059cd787995571ba92f75dc07bad8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reminderView = await graphClient.Me
    .ReminderView("2017-06-05T10:00:00.0000000","2017-06-11T11:00:00.0000000")
    .Request()
    .GetAsync();

```