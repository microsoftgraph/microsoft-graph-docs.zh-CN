---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d185da2dcde19e438c3a800e5cb8d8e6061d9ff
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarPermission()
role := "write"
requestBody.SetRole(&role)
options := &msgraphsdk.CalendarPermissionRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
calendarPermissionId := "calendarPermission-id"
graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Patch(options)


```