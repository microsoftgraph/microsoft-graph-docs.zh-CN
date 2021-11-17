---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa81aee74a2da5af6752656212b2fca74bd0afdd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024134"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
options := &msgraphsdk.FavoriteRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().Favorite().Post(options)


```