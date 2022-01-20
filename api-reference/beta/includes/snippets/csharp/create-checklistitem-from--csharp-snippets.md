---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24a858768977ee7e09b5533be18b2d0e058b4839
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItem = new ChecklistItem
{
    DisplayName = "Final sign-off from the team"
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].ChecklistItems
    .Request()
    .AddAsync(checklistItem);

```