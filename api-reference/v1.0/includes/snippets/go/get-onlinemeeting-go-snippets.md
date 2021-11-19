---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a546488189a57ae7a01a0b4a1e4a9a5b5870ef8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OnlineMeetingsRequestBuilderGetQueryParameters{
    Filter: "VideoTeleconferenceId%20eq%20'123456789'",
}
options := &msgraphsdk.OnlineMeetingsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Communications().OnlineMeetings().Get(options)


```