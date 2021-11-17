---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3352baca72056a98ddc346d7321e0672c097d65
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021992"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RegistrationRequestBuilderGetQueryParameters{
    Expand: "customQuestions",
}
options := &msgraphsdk.RegistrationRequestBuilderGetOptions{
    Q: requestParameters,
}
onlineMeetingId := "onlineMeeting-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Get(options)


```