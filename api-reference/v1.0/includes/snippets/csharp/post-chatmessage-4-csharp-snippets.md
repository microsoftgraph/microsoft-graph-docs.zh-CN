---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f80f920d791fea3e6ee7dc8394976b6e60626e82ebb280fbe374e65dcec42e6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    Attachments = new List<ChatMessageAttachment>()
    {
        new ChatMessageAttachment
        {
            Id = "153fa47d-18c9-4179-be08-9879815a9f90",
            ContentType = "reference",
            ContentUrl = "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            Name = "Budget.docx"
        }
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```