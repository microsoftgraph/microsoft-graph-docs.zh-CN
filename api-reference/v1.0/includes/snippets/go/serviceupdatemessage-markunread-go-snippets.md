---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d334dc3b6b13646f0d56c2a6167a76b87eb215a1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326314"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessageIdsRequestBody()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().MarkUnread().Post(requestBody)


```