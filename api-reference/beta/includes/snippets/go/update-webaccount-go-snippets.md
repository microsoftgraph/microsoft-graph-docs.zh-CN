---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bad6658ca3a5663b121914c092529737ab67934f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328820"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWebAccount()
webUrl := "https://github.com/innocenty.popov"
requestBody.SetWebUrl(&webUrl)
webAccountId := "webAccount-id"
graphClient.Me().Profile().WebAccountsById(&webAccountId).Patch(requestBody)


```