---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f9a81dfe8df0e151d46d07db4056d20516e66f5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975919"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ChatsRequestBuilderGetQueryParameters{
    Expand: "members",
    Filter: "members/any(o:%20o/displayname%20eq%20'Peter%20Parker')",
}
options := &msgraphsdk.ChatsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().Get(options)


```