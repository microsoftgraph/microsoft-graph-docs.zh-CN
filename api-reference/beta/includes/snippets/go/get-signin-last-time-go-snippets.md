---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f03c772a5d23b2f0c1bff3aa5573dd20e879976f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009720"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "displayName,userPrincipalName,signInActivity",
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Get(options)


```