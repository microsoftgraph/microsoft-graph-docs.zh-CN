---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9bf1c9c00f7c840b1d4c8e39a9fe6a180e3e92c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098782"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GetAllMessagesRequestBuilderGetQueryParameters{
    Top: 2,
}
options := &msgraphsdk.GetAllMessagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().GetAllMessages()(user-id).GetWithRequestConfigurationAndResponseHandler(options, nil)


```