---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea127f6b2ffc6989d326bc23355e3d062c60d287
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027441"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```