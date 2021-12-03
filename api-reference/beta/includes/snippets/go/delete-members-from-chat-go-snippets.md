---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b0be2ceee1449e9e4a067409423737af0cbe6a7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287921"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
conversationMemberId := "conversationMember-id"
graphClient.ChatsById(&chatId).MembersById(&conversationMemberId).Delete(nil)


```