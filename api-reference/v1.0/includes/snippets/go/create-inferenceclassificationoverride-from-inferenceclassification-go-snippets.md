---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 428c9762b321405080b8a6b45f57cb65726cb270
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097713"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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