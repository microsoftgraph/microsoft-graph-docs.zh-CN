---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7506b512122f9b2b69e7ef69c1bc4da9fded1c89
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
};

await graphClient.Me.Events["AAMkAGI1AAAt9AHjAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```