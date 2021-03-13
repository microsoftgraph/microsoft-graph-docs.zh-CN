---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c5a4a4aeaca7aa224ae9cbe42473ccaba471a1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"]
    .Request()
    .DeleteAsync();

```