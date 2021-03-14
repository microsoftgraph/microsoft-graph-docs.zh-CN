---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96c585c65d7082ce1e305dc1b9e8d4370be775a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"]
    .Request()
    .DeleteAsync();

```