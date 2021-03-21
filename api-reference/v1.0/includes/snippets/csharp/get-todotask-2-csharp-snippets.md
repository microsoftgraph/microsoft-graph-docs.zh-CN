---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a44689bd4d56f9d8d4cd01f9a1788650edb810
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963371"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks
    .Request()
    .GetAsync();

```