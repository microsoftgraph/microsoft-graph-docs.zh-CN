---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64433c5720a20b3e6d9a5b45e9569a306d879eb1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].LinkedResources["{linkedResource-id}"]
    .Request()
    .DeleteAsync();

```