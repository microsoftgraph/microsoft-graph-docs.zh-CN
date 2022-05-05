---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a899dc3e943ca6d75a127f031743610ed4eb033
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var simulationAutomations = await graphClient.Security.AttackSimulation.SimulationAutomations
    .Request()
    .GetAsync();

```