---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22be26f44d7dbf748d642c2954e06234762c654e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411619"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserIdsRequestBody()
requestBody.SetUserIds( []String {
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471",
}
options := &msgraphsdk.ConfirmCompromisedRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.IdentityProtection().RiskyUsers().ConfirmCompromised().Post(options)


```