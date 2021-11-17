---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07f8d1f06fe58aa053815ea8856dcfd1ee2a42c7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032836"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
swapShiftsChangeRequestId := "swapShiftsChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SwapShiftsChangeRequestsById(&swapShiftsChangeRequestId).Get(options)


```