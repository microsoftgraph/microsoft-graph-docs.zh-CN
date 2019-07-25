---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 92b10428b2e42c1cd6c992ae9d13c5c05a3777e2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728950"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Charity work"
};

await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAhrbPWAAA="]
    .Request()
    .UpdateAsync(outlookTaskFolder);

```