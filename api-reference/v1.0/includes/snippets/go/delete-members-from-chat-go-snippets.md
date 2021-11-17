---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdb1354ec521e4a5ccd807571800e06dfc76e384
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993683"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
conversationMemberId := "conversationMember-id"
graphClient.ChatsById(&chatId).MembersById(&conversationMemberId).Delete(options)


```