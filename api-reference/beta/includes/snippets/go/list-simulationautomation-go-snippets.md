---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d3c21e1c0b1a8ff602c86ccf01872fc2811a22c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203609"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Security().AttackSimulation().SimulationAutomations().Get(nil)


```