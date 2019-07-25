---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27310935ac5bee281f55e1d70e572e5e911895cd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = new OutlookTaskGroup
{
    Name = "Personal Tasks"
};

await graphClient.Me.Outlook.TaskGroups["AAMkADIyAAAhrbe-AAA="]
    .Request()
    .UpdateAsync(outlookTaskGroup);

```