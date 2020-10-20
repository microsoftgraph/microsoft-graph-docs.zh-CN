---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a7367dd63b34c9c530ed27985cfa1cb7335fdfa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Volunteer"
};

await graphClient.Me.Outlook.TaskFolders
    .Request()
    .AddAsync(outlookTaskFolder);

```