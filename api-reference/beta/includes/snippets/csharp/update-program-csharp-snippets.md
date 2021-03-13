---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84cc02543cedcbc59ddc550396dd55041751ef31
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803972"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var program = new Program
{
    DisplayName = "testprogram3 new name"
};

await graphClient.Programs["{program-id}"]
    .Request()
    .UpdateAsync(program);

```