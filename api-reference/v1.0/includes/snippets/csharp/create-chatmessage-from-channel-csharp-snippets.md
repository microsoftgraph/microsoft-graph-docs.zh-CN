---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 473f18c6b3a10e19e45c090bcf7f0964f9cbd81e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783602"
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