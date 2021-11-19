---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 088c1a52da2072ace60080ef73c4fa2c66f703e7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099892"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
swapShiftsChangeRequestId := "swapShiftsChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SwapShiftsChangeRequestsById(&swapShiftsChangeRequestId).Get(options)


```