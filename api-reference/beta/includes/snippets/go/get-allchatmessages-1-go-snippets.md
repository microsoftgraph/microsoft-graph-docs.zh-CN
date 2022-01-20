---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcce56e6455dd67757d38929e3408f73b024cdab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100539"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Top: 2,
    OrderBy: "createdDateTime",
}
options := &msgraphsdk.MessagesRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Messages().Get(options)


```