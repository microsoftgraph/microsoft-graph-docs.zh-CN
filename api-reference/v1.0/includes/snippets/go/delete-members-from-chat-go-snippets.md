---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cfc4aed382fcbc845a112d58b32be503088189d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
conversationMemberId := "conversationMember-id"
graphClient.ChatsById(&chatId).MembersById(&conversationMemberId).Delete(options)


```