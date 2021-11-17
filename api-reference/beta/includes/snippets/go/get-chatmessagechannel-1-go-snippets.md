---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d0103256edb7e45e0924119b6a158988ba21038
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).Get(options)


```