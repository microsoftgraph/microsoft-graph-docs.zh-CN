---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff1a92bf94d07d42681f1657f10d8b0c3c5548d9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994600"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.ChatsById(&chatId).MembersById(&conversationMemberId).Get(options)


```