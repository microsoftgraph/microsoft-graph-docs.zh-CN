---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b25a652398d4fe3c0bbf27dabaa914dfeaa57987
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326303"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOnlineMeeting()
startDateTime, err := time.Parse(time.RFC3339, "2019-07-12T14:30:34.2444915-07:00")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-07-12T15:00:34.2464912-07:00")
requestBody.SetEndDateTime(&endDateTime)
subject := "User Token Meeting"
requestBody.SetSubject(&subject)
result, err := graphClient.Me().OnlineMeetings().Post(requestBody)


```