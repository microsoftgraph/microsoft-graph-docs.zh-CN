---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf27233ea838af52a14f99f381cd2a990cad78da
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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