---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71f96ce8314c920e7b1f4c8b613718f011a31266
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendar()
name := "Marketing calendar"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarsRequestBuilderPostOptions{
    Body: requestBody,
}
calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Calendars().Post(options)


```