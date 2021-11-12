---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 897d86c8f390d2c19b0703f3bdeac5d6f8c9cbcb8e911bed045ba10bb7ebd7b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Cooking"
};

await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"].TaskFolders
    .Request()
    .AddAsync(outlookTaskFolder);

```