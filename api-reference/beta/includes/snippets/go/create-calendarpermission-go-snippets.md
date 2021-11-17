---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 846b8c5aeb0308ae3dbe99394a3b6b461fa2dc81
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012570"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCalendarPermission()
emailAddress := msgraphsdk.NewEmailAddress()
requestBody.SetEmailAddress(emailAddress)
name := "Samantha Booth"
emailAddress.SetName(&name)
address := "samanthab@adatum.onmicrosoft.com"
emailAddress.SetAddress(&address)
isInsideOrganization := true
requestBody.SetIsInsideOrganization(&isInsideOrganization)
isRemovable := true
requestBody.SetIsRemovable(&isRemovable)
role := "read"
requestBody.SetRole(&role)
options := &msgraphsdk.CalendarPermissionsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Calendar().CalendarPermissions().Post(options)


```