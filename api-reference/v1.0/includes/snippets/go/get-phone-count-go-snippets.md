---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10c393f955997709cfba92b29ad13dcb6f28cea1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ContactsRequestBuilderGetQueryParameters{
    Search: "%22displayName:wa%22",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ContactsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Contacts().Get(options)


```