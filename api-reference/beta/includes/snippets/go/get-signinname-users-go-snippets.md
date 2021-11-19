---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4a9ef4c2489cddc6bf01b6f4e113dd96d8c4077
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "displayName,id",
    Filter: "identities/any(c:c/issuerAssignedId%20eq%20'j.smith@yahoo.com'%20and%20c/issuer%20eq%20'contoso.onmicrosoft.com')",
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Get(options)


```