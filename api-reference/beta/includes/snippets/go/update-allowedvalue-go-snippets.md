---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e541e23f0c78f2f16e7bebcd5b5f0f9b90d5aa0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223957"
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
graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).AllowedValuesById(&allowedValueId).Patch(options)


```