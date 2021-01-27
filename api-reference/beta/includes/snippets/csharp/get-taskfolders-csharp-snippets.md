---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b5ea7a177e57a9b5a6cf98e1a2ffa4c5df6bcf4
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskGroups["AAMkADIyAAAhrbe-AAA="].TaskFolders
    .Request()
    .GetAsync();

```