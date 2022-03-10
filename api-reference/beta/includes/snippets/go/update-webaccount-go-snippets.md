---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7433ef3e326ecbdaa2861982337e5ce97911ed8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWebAccount()
webUrl := "https://github.com/innocenty.popov"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.WebAccountRequestBuilderPatchOptions{
    Body: requestBody,
}
webAccountId := "webAccount-id"
result, err := graphClient.Me().Profile().WebAccountsById(&webAccountId).Patch(options)


```