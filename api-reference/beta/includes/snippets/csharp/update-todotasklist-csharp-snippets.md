---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10cb237494578d82547cdaaf2f6e07fc534c8538
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = new TodoTaskList
{
    DisplayName = "Vacation Plan"
};

await graphClient.Me.Todo.Lists["AAMkADIyAAAhrbPWAAA="]
    .Request()
    .UpdateAsync(todoTaskList);

```