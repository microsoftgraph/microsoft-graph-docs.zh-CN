---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cab5ba8631fe39579ca05a7c77f7a6eca16d7fcd
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
mentionId := "mention-id"
result, err := graphClient.Me().MessagesById(&messageId).MentionsById(&mentionId).Delete(nil)


```