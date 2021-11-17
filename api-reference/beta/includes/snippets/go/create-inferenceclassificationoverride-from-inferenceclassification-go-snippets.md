---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055a91c5a187269653710fe2c2084ce917f91de5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974850"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewInferenceClassificationOverride()
classifyAs := "focused"
requestBody.SetClassifyAs(&classifyAs)
senderEmailAddress := msgraphsdk.NewEmailAddress()
requestBody.SetSenderEmailAddress(senderEmailAddress)
name := "Samantha Booth"
senderEmailAddress.SetName(&name)
address := "samanthab@adatum.onmicrosoft.com"
senderEmailAddress.SetAddress(&address)
options := &msgraphsdk.OverridesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().InferenceClassification().Overrides().Post(options)


```