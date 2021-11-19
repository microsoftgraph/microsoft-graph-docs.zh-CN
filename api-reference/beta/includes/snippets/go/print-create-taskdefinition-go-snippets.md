---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f46e1db445774b5f4d2e33beeb853b28de82d26e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081592"
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
options := &msgraphsdk.TaskDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Print().TaskDefinitions().Post(options)


```