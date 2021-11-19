---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5090fd60843ed03822509309e9dc73be107b74c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097859"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
mentionId := "mention-id"
graphClient.Me().MessagesById(&messageId).MentionsById(&mentionId).Delete(options)


```