---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 291e2bdfcda8036a36e813a838eaf794150107a6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412463"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "fd1c7836-4d84-4e24-b6aa-23188688cc54"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.SubscribeToToneRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).SubscribeToTone(call-id).Post(options)


```