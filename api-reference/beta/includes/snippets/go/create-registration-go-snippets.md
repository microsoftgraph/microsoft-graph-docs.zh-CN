---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8c88c57858edcefd5ff2ce6b4c7907b696e909a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137647"
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
options := &msgraphsdk.RegistrationRequestBuilderPostOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Post(options)


```