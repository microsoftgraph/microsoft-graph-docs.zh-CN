---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a2b611bc2292bf6cc29d7b6a90492de3c39c977
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994985"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
longRunningOperationId := "longRunningOperation-id"
result, err := graphClient.UsersById(&userId).Authentication().OperationsById(&longRunningOperationId).Get(options)


```