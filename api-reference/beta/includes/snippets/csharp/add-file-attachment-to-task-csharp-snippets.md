---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ffc0707372a19494b4bdec07a6e73ce7225f204
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = Encoding.ASCII.GetBytes("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
};

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```