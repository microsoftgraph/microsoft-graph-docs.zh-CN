---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aae8ce6ac4d8d0c51a0c3bd23f6f1ae9027a8c2
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Chats["{chat-id}"].Operations
    .Request()
    .GetAsync();

```