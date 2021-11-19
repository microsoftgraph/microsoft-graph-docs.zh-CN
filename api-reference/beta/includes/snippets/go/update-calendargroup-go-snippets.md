---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d51448dfaeca1597eafd9beade777ada454f82c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086924"
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
graphClient.Me().CalendarGroupsById(&calendarGroupId).Patch(options)


```