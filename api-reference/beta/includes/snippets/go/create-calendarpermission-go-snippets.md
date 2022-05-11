---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad900049298e2d6d88c3bae13abf24b18558173c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328112"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
userId := "user-id"
result, err := graphClient.UsersById(&userId).Calendar().CalendarPermissions().Post(requestBody)


```