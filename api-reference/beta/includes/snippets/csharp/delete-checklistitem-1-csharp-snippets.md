---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b5337249ca7844a66690001351fd671db8dd572
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66436743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].ChecklistItems["{checklistItem-id}"]
    .Request()
    .DeleteAsync();

```