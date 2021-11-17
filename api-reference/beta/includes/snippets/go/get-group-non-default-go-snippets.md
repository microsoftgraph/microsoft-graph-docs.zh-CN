---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dd2c4e0f97b7cf4ea40b967b7676d35d92b290c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015399"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount",
}
options := &msgraphsdk.GroupRequestBuilderGetOptions{
    Q: requestParameters,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Get(options)


```