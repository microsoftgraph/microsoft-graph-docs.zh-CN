---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b704bb1f7c810d58520b793e2f6a791d9750b290
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032878"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printOperationId := "printOperation-id"
result, err := graphClient.Print().OperationsById(&printOperationId).Get(options)


```