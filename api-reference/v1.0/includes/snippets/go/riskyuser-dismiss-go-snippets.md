---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a30c59a9bfa677f90a10103f8d05aa8f04481458
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088009"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetUserIds( []String {
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345",
}
options := &msgraphsdk.DismissRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.IdentityProtection().RiskyUsers().Dismiss().Post(options)


```