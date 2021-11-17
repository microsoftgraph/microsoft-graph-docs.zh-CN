---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2944c91e8e600fe9a2a2ac12525274709b35abf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UserRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mobilePhone",
}
options := &msgraphsdk.UserRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Get(options)


```