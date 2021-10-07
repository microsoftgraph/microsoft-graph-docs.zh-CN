---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bec305f2cebdf74fec2409ed5be5dd14668f593f
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAllMessages = await graphClient.Users["{user-id}"].Chats
    .GetAllMessages()
    .Request()
    .Top(2)
    .GetAsync();

```