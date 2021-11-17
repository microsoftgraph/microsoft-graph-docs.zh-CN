---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a470a6cdd0afacf8bdcba63f4c3762628bf5e0df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017960"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
teamsAsyncOperationId := "teamsAsyncOperation-id"
result, err := graphClient.ChatsById(&chatId).OperationsById(&teamsAsyncOperationId).Get(options)


```