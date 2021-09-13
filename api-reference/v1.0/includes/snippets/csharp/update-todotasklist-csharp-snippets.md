---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3cba80e1ca79845014d0144501525d1cb155a9e2c0f0b9b926fc56ed008443
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219622"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = new TodoTaskList
{
    DisplayName = "Vacation Plan"
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"]
    .Request()
    .UpdateAsync(todoTaskList);

```