---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa1d173cda94c61d3bee6c46dabad82dd1b984e8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022692"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCalendarGroup()
name := "name-value"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
calendarGroupId := "calendarGroup-id"
graphClient.Me().CalendarGroupsById(&calendarGroupId).Patch(options)


```