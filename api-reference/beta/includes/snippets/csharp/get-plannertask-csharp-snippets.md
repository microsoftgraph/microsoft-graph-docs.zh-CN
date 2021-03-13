---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c51b7477d172146bec16d0823dc2690c7ac07f30
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = await graphClient.Planner.Tasks["{plannerTask-id}"]
    .Request()
    .GetAsync();

```