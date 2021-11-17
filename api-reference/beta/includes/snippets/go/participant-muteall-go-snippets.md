---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed18ced8ebf78cf317752d517b9cddbc60d1447f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetParticipants( []String {
    "",
}
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.MuteAllRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Participants().MuteAll().Post(options)


```