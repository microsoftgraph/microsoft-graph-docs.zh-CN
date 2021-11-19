---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e657a499b6ac5b14a5129be9ebeb06fd525cf51d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085086"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TabsRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
}
options := &msgraphsdk.TabsRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Tabs().Get(options)


```