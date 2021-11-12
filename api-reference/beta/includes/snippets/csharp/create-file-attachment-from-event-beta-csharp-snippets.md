---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f46434ee64aefd15d4aad3ad1073f66ec027a527078772bd7042fdeef07bf75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = Encoding.ASCII.GetBytes("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
};

await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```