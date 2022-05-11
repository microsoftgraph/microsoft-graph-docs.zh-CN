---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db567decb49a19fcc67a2f6bec714908ecfac21e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327426"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
shiftId := "shift-id"
result, err := graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Get()


```