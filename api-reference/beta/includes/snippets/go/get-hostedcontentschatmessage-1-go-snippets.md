---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3391ffd1bb46a11a630871ca41e9a282a66f3923
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContents().Get(options)


```