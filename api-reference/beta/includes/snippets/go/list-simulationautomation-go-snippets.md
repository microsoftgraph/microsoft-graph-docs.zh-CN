---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d4afa752743147e2c7ac31abe0c1386e40a03a4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327205"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Security().AttackSimulation().SimulationAutomations().Get()


```