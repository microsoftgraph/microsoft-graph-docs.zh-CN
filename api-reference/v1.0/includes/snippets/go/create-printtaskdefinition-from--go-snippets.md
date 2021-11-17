---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 182cce35ac22f7ad7c4954a3c8368d5404cbef2a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003547"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrintTaskDefinition()
displayName := "Test TaskDefinitionName"
requestBody.SetDisplayName(&displayName)
createdBy := msgraphsdk.NewAppIdentity()
requestBody.SetCreatedBy(createdBy)
displayName := "Requesting App Display Name"
createdBy.SetDisplayName(&displayName)
options := &msgraphsdk.TaskDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Print().TaskDefinitions().Post(options)


```