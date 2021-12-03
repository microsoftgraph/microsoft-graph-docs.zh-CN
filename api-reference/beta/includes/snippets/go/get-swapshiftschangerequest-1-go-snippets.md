---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eefc5203b41b7d02a03277afac46ec0e9ebf0b20
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288304"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
swapShiftsChangeRequestId := "swapShiftsChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SwapShiftsChangeRequestsById(&swapShiftsChangeRequestId).Get(nil)


```