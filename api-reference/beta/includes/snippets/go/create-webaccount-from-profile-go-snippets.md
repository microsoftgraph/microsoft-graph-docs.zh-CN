---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593fbcc23a7fb26fd0857e4234faa1d5485fb3e4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023637"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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