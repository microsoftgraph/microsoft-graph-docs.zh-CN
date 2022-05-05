---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad8cfbf52311b079281948a8c9393d60ab34717b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var runs = await graphClient.Security.AttackSimulation.SimulationAutomations["{simulationAutomation-id}"].Runs
    .Request()
    .GetAsync();

```