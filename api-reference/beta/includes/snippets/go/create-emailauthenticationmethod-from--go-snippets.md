---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ba8fcaa8e9c19ab53e64d965ac3e8d50bed9e0d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEmailAuthenticationMethod()
emailAddress := "kim@contoso.com"
requestBody.SetEmailAddress(&emailAddress)
userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().EmailMethods().Post(requestBody)


```