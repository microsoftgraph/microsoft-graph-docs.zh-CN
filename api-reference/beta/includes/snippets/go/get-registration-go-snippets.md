---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ec93a26dbb1d7879a834576d2392a0d8cf14cc9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102103"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RegistrationRequestBuilderGetQueryParameters{
    Expand: "customQuestions",
}
options := &msgraphsdk.RegistrationRequestBuilderGetOptions{
    Q: requestParameters,
}
onlineMeetingId := "onlineMeeting-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Get(options)


```