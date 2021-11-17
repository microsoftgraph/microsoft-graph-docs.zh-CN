---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97f78be53ce0ace149dcc4030f3edf664f036b58
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCalendar()
name := "Volunteer"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Calendars().Post(options)


```