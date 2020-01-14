---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51291d8361ee315f00865be9b8f26f1ef098c840
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
};

await graphClient.Me.Outlook.Tasks["AAMkADAAAANXbdnAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```