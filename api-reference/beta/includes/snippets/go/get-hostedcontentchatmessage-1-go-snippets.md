---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 575e096b63ec094353bb18eece04ba1c556ad31f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
chatMessageHostedContentId := "chatMessageHostedContent-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContentsById(&chatMessageHostedContentId).Get(nil)


```