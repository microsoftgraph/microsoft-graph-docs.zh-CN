---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d33b86311fd260ac85660ac98b5bc3d82494bc06
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904430"
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