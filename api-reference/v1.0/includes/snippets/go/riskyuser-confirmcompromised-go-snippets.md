---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2d2e08f6e0e6b526219e7606906e3818a8d6bda
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088190"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetUserIds( []String {
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471",
}
options := &msgraphsdk.ConfirmCompromisedRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.IdentityProtection().RiskyUsers().ConfirmCompromised().Post(options)


```