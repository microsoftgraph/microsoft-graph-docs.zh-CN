---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3da86b6b35b0a37c6e2934929a8914662a15f7e7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printTaskDefinitionId := "printTaskDefinition-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Get(options)


```