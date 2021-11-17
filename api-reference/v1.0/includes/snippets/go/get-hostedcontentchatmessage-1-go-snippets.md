---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ebe75d73d129982db335de3d971e221d51cfb86
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
chatMessageId := "chatMessage-id"
chatMessageHostedContentId := "chatMessageHostedContent-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContentsById(&chatMessageHostedContentId).Get(options)


```