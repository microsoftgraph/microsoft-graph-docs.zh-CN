---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e64b20c35b87c39715e68a3d8745c66768c2b1ea
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087588"
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
result, err := graphClient.Communications().CallsById(&callId).UpdateRecordingStatus().Post(options)


```