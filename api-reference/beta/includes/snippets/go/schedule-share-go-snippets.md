---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 588263fb2764a7af285183c6a5c90afd127a5a25
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091817"
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
graphClient.TeamsById(&teamId).Schedule().Share().Post(options)


```