---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 80b16e5503041406e2765a8e24be4db527cbe314
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reminderView = await graphClient.Me
    .ReminderView("2017-06-05T10:00:00.0000000","2017-06-11T11:00:00.0000000")
    .Request()
    .GetAsync();

```