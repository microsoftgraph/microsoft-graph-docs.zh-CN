---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 023fbcf9ce3bfbc6a2506e064e097594940df3bc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks
    .Request()
    .GetAsync();

```