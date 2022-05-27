---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d31250ac71a1bdab831b9ec530ffa21f6cdc5fe
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719249"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserRequestBuilderGetQueryParameters{
    Count: true,
    OrderBy: "displayName",
    Search: "%22displayName:tier%22",
    Select: "displayName,id",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.UserRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).TransitiveMembers().User(group-id).GetWithRequestConfigurationAndResponseHandler(options, nil)


```