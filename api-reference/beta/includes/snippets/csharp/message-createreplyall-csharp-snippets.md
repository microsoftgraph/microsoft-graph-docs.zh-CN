---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adc7da0a9057545d6966a816f42789f9e56d4162cf3556f6f4ef5cd22ce54e70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220640"
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