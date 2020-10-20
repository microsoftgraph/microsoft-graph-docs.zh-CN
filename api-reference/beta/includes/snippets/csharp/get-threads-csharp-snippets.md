---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b1035bb4fdff81b1eab92f59750532e2bee1f41
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{id}"].Conversations["{id}"].Threads
    .Request()
    .GetAsync();

```