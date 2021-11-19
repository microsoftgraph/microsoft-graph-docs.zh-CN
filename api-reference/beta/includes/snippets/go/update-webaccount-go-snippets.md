---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0c4b8854155d9d285100a5917499e628459e1e2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083909"
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
graphClient.Me().Profile().WebAccountsById(&webAccountId).Patch(options)


```