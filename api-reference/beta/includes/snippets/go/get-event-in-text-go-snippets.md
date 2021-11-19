---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a8b64565090f3a70a5c65e18d416d667280a2b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082830"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```