---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 252a395b2f014914b54b6a669893292f6bdb3e61
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083740"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendar()
name := "Volunteer"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Calendars().Post(options)


```