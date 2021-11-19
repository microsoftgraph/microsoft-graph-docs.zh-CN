---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87ad35d360a0fea668add70e815c5b8a5092d19c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086908"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
options := &msgraphsdk.GroupRequestBuilderGetOptions{
    Q: requestParameters,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Get(options)


```