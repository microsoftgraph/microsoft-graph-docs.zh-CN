---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb3a93d685165d40305e22f18004d665f2f1200f
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    Topic = "Group chat title update"
};

await graphClient.Chats["19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2"]
    .Request()
    .UpdateAsync(chat);

```