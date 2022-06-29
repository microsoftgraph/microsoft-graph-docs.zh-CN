---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a2318194e0991d65956b147fd2579d01a25c021
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695260"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].PinnedMessages["{pinnedChatMessageInfo-id}"]
    .Request()
    .DeleteAsync();

```