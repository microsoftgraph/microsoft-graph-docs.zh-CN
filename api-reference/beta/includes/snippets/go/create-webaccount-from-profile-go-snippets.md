---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc5c407ab0ca62be115fc726979db437e37332cd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326878"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWebAccount()
description := "My Github contributions!"
requestBody.SetDescription(&description)
userId := "innocenty.popov"
requestBody.SetUserId(&userId)
service := msgraphsdk.NewServiceInformation()
requestBody.SetService(service)
name := "GitHub"
service.SetName(&name)
webUrl := "https://github.com"
service.SetWebUrl(&webUrl)
result, err := graphClient.Me().Profile().WebAccounts().Post(requestBody)


```