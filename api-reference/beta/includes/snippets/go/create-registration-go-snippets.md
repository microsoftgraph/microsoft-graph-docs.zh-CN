---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 361312a132961d1f1a42943a76ce8ecc5723e8df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011723"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
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