---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbdd48ce360a3c46406f5fbe8448ffa61dd0fd9c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411983"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffId := "timeOff-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Delete(nil)


```