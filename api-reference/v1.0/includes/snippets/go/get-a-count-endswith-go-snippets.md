---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4873bb6cb395e8a0de8e263b8d91d5f2f8a7df72
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082966"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Filter: "endswith(mail,'a@contoso.com')",
    Orderby: "userPrincipalName",
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