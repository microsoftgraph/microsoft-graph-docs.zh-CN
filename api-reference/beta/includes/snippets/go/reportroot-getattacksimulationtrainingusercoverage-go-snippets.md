---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b66f6ea8d1bbbbfabe99f117d2a57a07c6f5b51
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328146"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().GetAttackSimulationTrainingUserCoverage()().Get()


```