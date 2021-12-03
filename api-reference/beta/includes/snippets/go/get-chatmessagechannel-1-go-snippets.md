---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ebbe359757c62d1cbd88abd81181b7ed50893c9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287909"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).Get(nil)


```