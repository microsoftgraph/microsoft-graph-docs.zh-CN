---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff51031bf9b41bf0eaa971319b69c9c549cc9b19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013410"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetEmailAddresses( []String {
    "danas@contoso.onmicrosoft.com",
    "fannyd@contoso.onmicrosoft.com",
}
mailTipsOptions := "automaticReplies, mailboxFullStatus"
requestBody.SetMailTipsOptions(&mailTipsOptions)
options := &msgraphsdk.GetMailTipsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().GetMailTips().Post(options)


```