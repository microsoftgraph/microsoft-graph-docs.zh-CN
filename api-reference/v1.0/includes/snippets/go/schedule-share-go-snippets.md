---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de420629c1f49abd1b37e720354c84fa18f4f6e7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411708"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
notifyTeam := true
requestBody.SetNotifyTeam(&notifyTeam)
startDateTime, err := time.Parse(time.RFC3339, "2018-10-08T00:00:00.000Z")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-10-15T00:00:00.000Z")
requestBody.SetEndDateTime(&endDateTime)
options := &msgraphsdk.ShareRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Share(team-id).Post(options)


```