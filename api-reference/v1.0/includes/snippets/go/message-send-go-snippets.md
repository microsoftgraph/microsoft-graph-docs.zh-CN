---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f5444e2098add01fb7613f7ae47288ba18865be
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Send().Post(options)


```