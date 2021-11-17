---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bc34f074573a8887d20de98e8769f0d0a2be86c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000137"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
conversationId := "conversation-id"
graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Delete(options)


```