---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 180eb0bc6c40df3b6a08385c8da7448325473c29
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItems = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].ChecklistItems
    .Request()
    .GetAsync();

```