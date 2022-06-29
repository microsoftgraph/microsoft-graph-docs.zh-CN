---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16ab2039788cf07eabc355057eeb9bf8f06a86f2
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66440765"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItem = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].ChecklistItems["{checklistItem-id}"]
    .Request()
    .GetAsync();

```