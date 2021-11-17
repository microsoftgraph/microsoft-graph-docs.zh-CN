---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bef704bbbc0e354cb8530460c15a5b9534e57655
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975916"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ChatsRequestBuilderGetQueryParameters{
    Expand: "members",
}
options := &msgraphsdk.ChatsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().Get(options)


```