---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5ae34175dcc30e09906ef3adfff8b7f878d5a1c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090258"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount",
}
options := &msgraphsdk.GroupRequestBuilderGetOptions{
    Q: requestParameters,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Get(options)


```