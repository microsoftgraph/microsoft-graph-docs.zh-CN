---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 585acc4cda3166990cd7339986e4ae46aaf87bfb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096883"
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
graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).Patch(options)


```