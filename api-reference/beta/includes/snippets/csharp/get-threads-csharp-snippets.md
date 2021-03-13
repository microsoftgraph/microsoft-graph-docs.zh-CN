---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83a183bcd84383eaa1c77778d9bda6862566f3a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"].Threads
    .Request()
    .GetAsync();

```