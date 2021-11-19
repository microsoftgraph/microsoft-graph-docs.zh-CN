---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78f743e52cb48fd4c10d1b62c895c27f3ae90c18
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091568"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventsRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,organizer,attendees,start,end,location",
}
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.EventsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Me().Events().Get(options)


```