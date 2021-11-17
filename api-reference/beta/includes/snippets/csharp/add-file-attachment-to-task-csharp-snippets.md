---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 786e8d0e6767be6574deeffd541500853e231d4a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = Convert.FromBase64String("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
};

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```