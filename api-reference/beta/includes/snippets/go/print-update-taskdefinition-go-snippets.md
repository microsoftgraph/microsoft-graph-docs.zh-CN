---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f75bc79070877c68c37254ce10588be5f16a3aaa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099200"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrintTaskDefinition()
displayName := "Test TaskDefinitionName"
requestBody.SetDisplayName(&displayName)
createdBy := msgraphsdk.NewAppIdentity()
requestBody.SetCreatedBy(createdBy)
displayName := "Requesting App Display Name"
createdBy.SetDisplayName(&displayName)
options := &msgraphsdk.PrintTaskDefinitionRequestBuilderPatchOptions{
    Body: requestBody,
}
printTaskDefinitionId := "printTaskDefinition-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Patch(options)


```