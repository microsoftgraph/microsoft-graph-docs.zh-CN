---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50dfddd609b110d570685a1286fa3737d333a61f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TabsRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
}
options := &msgraphsdk.TabsRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Tabs().Get(options)


```