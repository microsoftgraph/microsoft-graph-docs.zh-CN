---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c76393fbed46ab8873b3f3386c485659b9f57c63
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412224"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.CancelMediaProcessingRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).CancelMediaProcessing(call-id).Post(options)


```