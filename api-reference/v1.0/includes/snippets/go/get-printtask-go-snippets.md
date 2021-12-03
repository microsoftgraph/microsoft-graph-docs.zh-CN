---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdf84cc611917d8a7c38aa70a426cdfa31003e25
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288824"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Get(nil)


```