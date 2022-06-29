---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e38fb5c61647d10548a699a231857a4068a75a7
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66436224"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItem = new ChecklistItem
{
    DisplayName = "buy cake"
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].ChecklistItems["{checklistItem-id}"]
    .Request()
    .UpdateAsync(checklistItem);

```