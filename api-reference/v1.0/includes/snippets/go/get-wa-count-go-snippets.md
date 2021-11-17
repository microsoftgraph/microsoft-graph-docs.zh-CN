---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ed58c26fdbbadd03a5b4b956c9d920c18a7af60
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992397"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Search: "%22displayName:wa%22",
    Orderby: "displayName",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Users().Get(options)


```