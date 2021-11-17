---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff0868a704a089c36768ff077e42e1fd04f651d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60987130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "Take your wellness days and rest",
    Posts = new ConversationThreadPostsCollectionPage()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "Waiting for the summer holidays."
            }
        }
    }
};

await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```