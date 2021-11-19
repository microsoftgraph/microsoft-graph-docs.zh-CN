---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68e9d8db2971c8581313b702ae5baf9b56a60c18
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086129"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.CancelMediaProcessingRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).CancelMediaProcessing().Post(options)


```