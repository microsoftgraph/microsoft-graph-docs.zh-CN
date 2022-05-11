---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd6c4e7b25d3ec3a6835d54882e6ae2dba3efd37
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327620"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

simulationAutomationId := "simulationAutomation-id"
result, err := graphClient.Security().AttackSimulation().SimulationAutomationsById(&simulationAutomationId).Runs().Get()


```