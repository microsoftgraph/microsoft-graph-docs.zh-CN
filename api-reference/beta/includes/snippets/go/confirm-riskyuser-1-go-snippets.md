---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dc3aa05c654caf5a553c428c43f6d53e96089be
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096048"
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
graphClient.RiskyUsers().ConfirmCompromised().Post(options)


```