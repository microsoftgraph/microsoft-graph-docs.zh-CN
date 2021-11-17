---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33cbb1000cd344f0dd5176f3551f4df50dec9967
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009898"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UserRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mobilePhone",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.UserRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Get(options)


```