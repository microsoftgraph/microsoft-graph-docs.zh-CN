---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fad5669374774597de99da3c0fe848a06b7b169e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{user-id}"].Chats["{chat-id}"]
    .Request()
    .GetAsync();

```