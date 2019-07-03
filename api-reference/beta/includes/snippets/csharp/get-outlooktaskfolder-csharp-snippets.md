---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 971545faba675f855c05a820df814d794222c319
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAAABrJAAA="]
    .Request()
    .GetAsync();

```