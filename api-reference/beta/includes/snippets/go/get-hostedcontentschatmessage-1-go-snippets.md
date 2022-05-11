---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ace0b4cfe6356f7657e8fddf0ad3252f9a9dd2d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328625"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContents().Get()


```