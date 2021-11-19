---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54135c7fe1f1f86be8172b28db04f36298e6bfd6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097861"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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