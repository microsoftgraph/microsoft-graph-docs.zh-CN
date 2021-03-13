---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b34c31f2d00db6f73592292ff0ac4926c125bbd0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Rosters["{plannerRoster-id}"]
    .Request()
    .DeleteAsync();

```