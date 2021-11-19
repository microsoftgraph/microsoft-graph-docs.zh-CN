---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c7a969866f7024559315b2dc8356bed06eb0d76
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100279"
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
options := &msgraphsdk.WebAccountsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().WebAccounts().Post(options)


```