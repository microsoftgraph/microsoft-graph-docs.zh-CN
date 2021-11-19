---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bef29279b8abcd933c91d95f05f7a473bafd3ac
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092669"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
conversationId := "conversation-id"
graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Delete(options)


```