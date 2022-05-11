---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 531a2d7db4aa63b6ce9e3051fbdfcae239e667fc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327340"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
chatMessageHostedContentId := "chatMessageHostedContent-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContentsById(&chatMessageHostedContentId).Get()


```