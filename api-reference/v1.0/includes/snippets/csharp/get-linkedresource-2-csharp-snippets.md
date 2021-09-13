---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52f3a32fffecd3eee7303e119c3b7b22ffd93fc6cf8ac011ffa3428e0fa1f2ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResources = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].LinkedResources
    .Request()
    .GetAsync();

```