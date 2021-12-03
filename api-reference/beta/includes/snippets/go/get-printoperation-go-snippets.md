---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d03301392efb6e723c62b26c29608dab0f2e1d0d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288029"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printOperationId := "printOperation-id"
result, err := graphClient.Print().OperationsById(&printOperationId).Get(nil)


```