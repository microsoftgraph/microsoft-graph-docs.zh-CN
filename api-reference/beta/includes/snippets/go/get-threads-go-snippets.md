---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 771250f31afc8aab837794d9da7f1fb5d7c1c225
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030426"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
conversationId := "conversation-id"
result, err := graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Threads().Get(options)


```