---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f19603856d2701c28bcc6048048ca8ede883664b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212668"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

simulationAutomationId := "simulationAutomation-id"
result, err := graphClient.Security().AttackSimulation().SimulationAutomationsById(&simulationAutomationId).Runs().Get(nil)


```