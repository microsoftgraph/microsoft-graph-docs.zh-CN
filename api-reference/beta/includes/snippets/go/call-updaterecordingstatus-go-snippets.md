---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb8f06492eae897f15e49dc181004e6d34ec1e1c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412064"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
status := "notRecording | recording | failed"
requestBody.SetStatus(&status)
options := &msgraphsdk.UpdateRecordingStatusRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).UpdateRecordingStatus(call-id).Post(options)


```