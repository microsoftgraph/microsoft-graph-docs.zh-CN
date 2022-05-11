---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5073d59667ba0e4714a1fd534f784b9150e1faea
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327676"
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
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Share(team-id).Post(requestBody)


```