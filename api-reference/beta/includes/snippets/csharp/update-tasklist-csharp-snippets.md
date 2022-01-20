---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5a2bb1b33934278628e006df7b5e20f4388ae2b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTaskList = new BaseTaskList
{
    DisplayName = "Travel Plan"
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"]
    .Request()
    .UpdateAsync(baseTaskList);

```