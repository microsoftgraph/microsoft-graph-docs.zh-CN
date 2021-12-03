---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc47e32456f58a7ba4a3b681dbfd6d8afe6a9a84
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287504"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
shiftId := "shift-id"
result, err := graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Get(nil)


```