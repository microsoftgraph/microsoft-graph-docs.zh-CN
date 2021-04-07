---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c1eb4f2f26b7eb1ffccc797d8f37e94c1eb8939
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        Content = "Hello world"
    }
};

await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```