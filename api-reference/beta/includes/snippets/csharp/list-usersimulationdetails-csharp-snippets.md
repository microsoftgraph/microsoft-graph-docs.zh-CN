---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23029d449c369aa4bfe1ec8e781e6feaf72b8751
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var simulations = await graphClient.Security.AttackSimulation.Simulations["{simulation-id}"]
    .Request()
    .Select("Report")
    .GetAsync();

var simulationUsers = simulations.Report.SimulationUsers;

```