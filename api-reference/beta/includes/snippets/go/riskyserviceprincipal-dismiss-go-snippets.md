---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 985d992b0babae18bb7d8ed9e80d5e00be3a69b2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327625"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipalIdsRequestBody()
requestBody.SetServicePrincipalIds( []String {
    "9089a539-a539-9089-39a5-899039a58990",
}
graphClient.IdentityProtection().RiskyServicePrincipals().Dismiss().Post(requestBody)


```