---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 971545faba675f855c05a820df814d794222c319
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAAABrJAAA="]
    .Request()
    .GetAsync();

```