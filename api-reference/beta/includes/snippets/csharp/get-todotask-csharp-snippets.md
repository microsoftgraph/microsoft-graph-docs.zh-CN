---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a44689bd4d56f9d8d4cd01f9a1788650edb810
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks
    .Request()
    .GetAsync();

```