---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d631fd9243d0426db245da4556abb5b52f89766
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411724"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarGroup()
name := "name-value"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Patch(options)


```