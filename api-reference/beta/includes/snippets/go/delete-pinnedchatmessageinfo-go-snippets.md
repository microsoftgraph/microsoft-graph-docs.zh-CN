---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 511d058b3760009e8e9cff8a341d05ffa4814f13
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695261"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
pinnedChatMessageInfoId := "pinnedChatMessageInfo-id"
graphClient.ChatsById(&chatId).PinnedMessagesById(&pinnedChatMessageInfoId).Delete()


```