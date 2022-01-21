---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16ab2039788cf07eabc355057eeb9bf8f06a86f2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItem = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].ChecklistItems["{checklistItem-id}"]
    .Request()
    .GetAsync();

```