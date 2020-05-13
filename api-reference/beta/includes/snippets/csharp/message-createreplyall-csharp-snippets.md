---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3287e286f0e9e5c91e7d41d4c5be51e3002e649
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "37544193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Attachments = new List<Attachment>()
    {
        new FileAttachment
        {
            Name = "guidelines.txt",
            ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
        }
    }
};

var comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaKAAA="]
    .CreateReplyAll(message,comment)
    .Request()
    .PostAsync();

```