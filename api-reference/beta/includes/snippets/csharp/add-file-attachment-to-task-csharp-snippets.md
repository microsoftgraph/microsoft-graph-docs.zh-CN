---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c8a4690d886fca8e28ba04f33515c578f6d7390
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684962"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = Encoding.ASCII.GetBytes("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
};

await graphClient.Me.Outlook.Tasks["AAMkADAAAANXbdnAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```