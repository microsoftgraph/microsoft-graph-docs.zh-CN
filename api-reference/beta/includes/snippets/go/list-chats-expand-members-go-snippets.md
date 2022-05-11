---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd8923d243a724bc73e53590b49667013822e8f6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327871"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatsRequestBuilderGetQueryParameters{
    Expand: "members",
}
options := &msgraphsdk.ChatsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().GetWithRequestConfigurationAndResponseHandler(options, nil)


```