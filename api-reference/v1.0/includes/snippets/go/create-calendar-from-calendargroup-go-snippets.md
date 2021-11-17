---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a350edfe9dd40cf6b66c3a28ea812243c548f1ac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000865"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCalendar()
name := "Marketing calendar"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarsRequestBuilderPostOptions{
    Body: requestBody,
}
calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Calendars().Post(options)


```