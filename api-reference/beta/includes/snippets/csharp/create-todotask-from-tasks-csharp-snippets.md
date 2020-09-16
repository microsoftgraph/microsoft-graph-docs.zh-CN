---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d33b86311fd260ac85660ac98b5bc3d82494bc06
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = new TodoTask
{
    Title = "A new task",
    LinkedResources = (ITodoTaskLinkedResourcesCollectionPage)new List<LinkedResource>()
    {
        new LinkedResource
        {
            WebUrl = "http://microsoft.com",
            ApplicationName = "Microsoft",
            DisplayName = "Microsoft"
        }
    }
};

await graphClient.Me.Todo.Lists["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"].Tasks
    .Request()
    .AddAsync(todoTask);

```