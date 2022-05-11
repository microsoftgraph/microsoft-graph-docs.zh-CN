---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e29a8c1438aba4fddada88882ca16901df92cf8d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329057"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
status := "notRecording | recording | failed"
requestBody.SetStatus(&status)
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).UpdateRecordingStatus(call-id).Post(requestBody)


```