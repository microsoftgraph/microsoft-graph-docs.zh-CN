---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63cb5efff3f8600f71ab363395c5cfa74c23ffd3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326587"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.meetingRegistration",
    "subject": "Microsoft Ignite",
    "description": "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.",
    "startDateTime": "2021-11-02T08:00:00-08:00",
    "endDateTime": "2021-11-04T04:00:00-08:00",
    "allowedRegistrant": "everyone",
    "speakers":  []Object {
    }
    "customQuestions":  []Object {
    }
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Post(requestBody)


```