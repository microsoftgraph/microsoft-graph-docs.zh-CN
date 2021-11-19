---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbc45d10212be7190277e38743f6e710271b805d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093638"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.GroupRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Get(options)


```