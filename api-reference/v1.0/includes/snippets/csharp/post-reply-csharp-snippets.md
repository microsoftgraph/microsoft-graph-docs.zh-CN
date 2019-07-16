---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ebb6dfce68b492f61780e13704477d741f5431e1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    ReceivedDateTime = "datetime-value",
    HasAttachments = true,
    From = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    Sender = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    ConversationThreadId = "conversationThreadId-value",
    NewParticipants = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "name-value",
                Address = "address-value"
            }
        }
    },
    ConversationId = "conversationId-value",
    CreatedDateTime = "datetime-value",
    LastModifiedDateTime = "datetime-value",
    ChangeKey = "changeKey-value",
    Categories = new List<String>()
    {
        "categories-value"
    },
    Id = "id-value",
    InReplyTo = new Post
    {
    },
    Attachments = new List<Attachment>()
    {
        new Attachment
        {
            LastModifiedDateTime = "datetime-value",
            Name = "name-value",
            ContentType = "contentType-value",
            Size = 99,
            IsInline = true,
            Id = "id-value"
        }
    }
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```