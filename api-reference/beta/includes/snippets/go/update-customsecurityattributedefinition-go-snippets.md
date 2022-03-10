---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddf752b735a6b276b1690a1611dce60e2240f212
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411764"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustomSecurityAttributeDefinition()
description := "Target completion date (YYYY/MM/DD)"
requestBody.SetDescription(&description)
options := &msgraphsdk.CustomSecurityAttributeDefinitionRequestBuilderPatchOptions{
    Body: requestBody,
}
customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
result, err := graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).Patch(options)


```