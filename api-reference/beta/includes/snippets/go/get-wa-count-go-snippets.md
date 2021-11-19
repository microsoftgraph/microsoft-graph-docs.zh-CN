---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47e86d199129cadc0491a83cbf0f76560857fe89
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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