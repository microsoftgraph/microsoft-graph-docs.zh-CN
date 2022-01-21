---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b760d0a5ebeafb8a3488494773d98a1f04cd8a8d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationTaskListId = "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG";

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"]
    .Move(destinationTaskListId)
    .Request()
    .PostAsync();

```