---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4d27945b972b07f5447e011df1a23eb5a20ee5eb4875b6f1ac0fa96cfcadb97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163387"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"].TaskFolders
    .Request()
    .GetAsync();

```