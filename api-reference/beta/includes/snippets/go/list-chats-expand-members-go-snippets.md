---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f38746dfd86e45076d789f4b9a29c08e1e927d36
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatsRequestBuilderGetQueryParameters{
    Expand: "members",
}
options := &msgraphsdk.ChatsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().Get(options)


```