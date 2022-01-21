---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b73f2adb4cb1ca09714abc122e4c5b845a6e38fa
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks
    .Delta()
    .Request()
    .GetAsync();

```