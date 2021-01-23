---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7ea0c66ca855def3c670fa61072d05b844045d7
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        Content = "Hello World"
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```