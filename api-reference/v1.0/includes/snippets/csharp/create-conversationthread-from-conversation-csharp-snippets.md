---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 576dd36793cfa22a3306f04acba5e700d62746194eca4b05b528c9bf92860986
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "topic-value",
    Posts = new ConversationThreadPostsCollectionPage()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "this is body content"
            }
        }
    }
};

await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```