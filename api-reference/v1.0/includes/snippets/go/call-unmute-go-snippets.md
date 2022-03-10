---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02fa5d5b04ab30b2186f4e3c63661b7dff4470d9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412217"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.UnmuteRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Unmute(call-id).Post(options)


```