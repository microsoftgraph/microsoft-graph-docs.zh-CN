---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e38e2e2a4110493cff3615841847a341f24dde26
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095070"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
conversationId := "conversation-id"
result, err := graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Threads().Get(options)


```