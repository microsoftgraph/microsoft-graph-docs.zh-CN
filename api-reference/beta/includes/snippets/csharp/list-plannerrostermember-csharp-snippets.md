---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c848313f56e4787a24fed6d6f5005bdbf23a63fc
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Planner.Rosters["6519868f-868f-6519-8f86-19658f861965"].Members
    .Request()
    .GetAsync();

```