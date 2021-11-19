---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ecd6ad9db9a3f0c5f1e76971f90f911bf98f174
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101094"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,'Eric')",
    Select: "displayName,signInActivity",
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Get(options)


```