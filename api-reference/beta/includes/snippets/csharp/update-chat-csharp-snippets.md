---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4428429f1ef0f93339389a382675b179db35621b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    Topic = "Group chat title update"
};

await graphClient.Chats["{chat-id}"]
    .Request()
    .UpdateAsync(chat);

```