---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3212b17083f1a3677e91cab76b281698e3752081
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItems = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].ChecklistItems
    .Request()
    .GetAsync();

```