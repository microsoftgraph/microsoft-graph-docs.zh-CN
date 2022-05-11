---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 035f46ca8334aa217a3933baabe840072a0262ac
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328783"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetEmailAddresses( []String {
    "danas@contoso.onmicrosoft.com",
    "fannyd@contoso.onmicrosoft.com",
}
mailTipsOptions := "automaticReplies, mailboxFullStatus"
requestBody.SetMailTipsOptions(&mailTipsOptions)
result, err := graphClient.Me().GetMailTips().Post(requestBody)


```