---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47cb09dbd1b326122fce7c44af5d4c5168c7a18f
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Attachments = (IMessageAttachmentsCollectionPage)new List<Attachment>()
    {
        new FileAttachment
        {
            Name = "guidelines.txt",
            ContentBytes = Encoding.ASCII.GetBytes("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
        }
    }
};

var comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaKAAA="]
    .CreateReplyAll(message,comment)
    .Request()
    .PostAsync();

```