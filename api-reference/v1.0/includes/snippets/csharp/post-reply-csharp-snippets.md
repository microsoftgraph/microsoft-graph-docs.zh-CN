---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c308d664e6488a66616d6a522af50a4366a869b
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945167"
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
    ReceivedDateTime = DateTimeOffset.Parse("datetime-value"),
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
    CreatedDateTime = DateTimeOffset.Parse("datetime-value"),
    LastModifiedDateTime = DateTimeOffset.Parse("datetime-value"),
    ChangeKey = "changeKey-value",
    Categories = new List<String>()
    {
        "categories-value"
    },
    Id = "id-value",
    InReplyTo = new Post
    {
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new Attachment
        {
            LastModifiedDateTime = DateTimeOffset.Parse("datetime-value"),
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