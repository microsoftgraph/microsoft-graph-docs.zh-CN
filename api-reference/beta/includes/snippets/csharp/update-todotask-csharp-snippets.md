---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86bf9c084873e16d81b531b1258ac8f83576234e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806489"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = new TodoTask
{
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2020-07-25T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"]
    .Request()
    .UpdateAsync(todoTask);

```