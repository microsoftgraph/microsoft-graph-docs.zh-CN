---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f9574f78c6c31ee808b7ff05cea898ad8dcde67
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093837"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printOperationId := "printOperation-id"
result, err := graphClient.Print().OperationsById(&printOperationId).Get(options)


```