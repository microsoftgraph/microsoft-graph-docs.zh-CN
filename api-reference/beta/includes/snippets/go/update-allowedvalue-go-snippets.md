---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18372a2ae6ed6d7add3d52d862d0d0fc43e42991
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAllowedValue()
isActive := "false"
requestBody.SetIsActive(&isActive)
options := &msgraphsdk.AllowedValueRequestBuilderPatchOptions{
    Body: requestBody,
}
customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
allowedValueId := "allowedValue-id"
result, err := graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).AllowedValuesById(&allowedValueId).Patch(options)


```