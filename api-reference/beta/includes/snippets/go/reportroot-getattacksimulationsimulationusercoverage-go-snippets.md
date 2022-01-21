---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 054af3d9ad6c471194b351f82e9191afaa344c8c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135077"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().GetAttackSimulationSimulationUserCoverage()().Get(nil)


```