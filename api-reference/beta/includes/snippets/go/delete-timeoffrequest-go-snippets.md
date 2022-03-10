---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc47c973d227aaf2f704bafb46711cd493bf1e39
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412708"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Delete(nil)


```