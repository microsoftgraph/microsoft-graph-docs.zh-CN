---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f629ca13ce9bec3bd57b376836cebf1b112b6ac
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66436740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].ChecklistItems["{checklistItem-id}"]
    .Request()
    .DeleteAsync();

```