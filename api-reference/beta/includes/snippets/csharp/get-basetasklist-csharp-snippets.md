---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2147241b86c88d36328f6690c50ac3e459df46c9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116621"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTaskList = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"]
    .Request()
    .GetAsync();

```