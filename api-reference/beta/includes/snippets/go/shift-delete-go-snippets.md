---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df715df258fc617d3d3b4bf0947c95180e669574
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020479"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
shiftId := "shift-id"
graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Delete(options)


```