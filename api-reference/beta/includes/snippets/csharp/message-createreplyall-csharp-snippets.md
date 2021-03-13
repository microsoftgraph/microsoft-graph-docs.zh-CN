---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff7c87f83423f88e0c238a6b77769ed194548d94
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Attachments = new MessageAttachmentsCollectionPage()
    {
        new FileAttachment
        {
            Name = "guidelines.txt",
            ContentBytes = Encoding.ASCII.GetBytes("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
        }
    }
};

var comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["{message-id}"]
    .CreateReplyAll(message,comment)
    .Request()
    .PostAsync();

```