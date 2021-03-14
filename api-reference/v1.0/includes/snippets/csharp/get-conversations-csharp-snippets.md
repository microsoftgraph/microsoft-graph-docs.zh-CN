---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80812f9e5ade751144434c8b86041651c8dfadd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversations = await graphClient.Groups["{group-id}"].Conversations
    .Request()
    .GetAsync();

```