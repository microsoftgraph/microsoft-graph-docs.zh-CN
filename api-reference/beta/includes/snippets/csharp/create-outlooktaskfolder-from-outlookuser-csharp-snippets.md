---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aa173df23f7a347025d889f8b4ad87b8e57ce39c7ff4127388d6d0d43d89725
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221308"
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