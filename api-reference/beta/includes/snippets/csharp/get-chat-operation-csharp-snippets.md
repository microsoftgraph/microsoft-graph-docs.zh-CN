---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e844496525450a8cbf04bedf6a11b4dd375dfc0
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAsyncOperation = await graphClient.Chats["{chat-id}"].Operations["{teamsAsyncOperation-id}"]
    .Request()
    .GetAsync();

```