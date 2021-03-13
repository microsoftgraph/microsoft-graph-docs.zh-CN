---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecdbf3586a03df92a3c7d375f73bfa80fda1a3e2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790705"
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

var comment = "Please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["{message-id}"]
    .ReplyAll(message,comment)
    .Request()
    .PostAsync();

```