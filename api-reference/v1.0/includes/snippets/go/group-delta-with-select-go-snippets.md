---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64f3987b155cc34124175f44caaae0f58c5d5c2f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000104"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
options := &msgraphsdk.GroupRequestBuilderGetOptions{
    Q: requestParameters,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Get(options)


```